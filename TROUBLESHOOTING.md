# Ayonix AI-MED Troubleshooting Guide

## Understanding the Ayonix AI-MED Architecture

The Ayonix AI-MED system is designed to streamline interactions between your browser and the AI-MED API. At the heart of this design is a backend reverse proxy, enhancing security and resolving CORS issues.

- **How it Works**: The Ayonix AI-MED is designed to interact with the AI-MED API through a specific route. When a request is made from the Webpage to AI-MED, it is not directly sent to the AI-MED API. Initially, the request is sent to the Ayonix AI-MED backend via `/AI-MED/api` route. From there, the backend is responsible for forwarding the request to the AI-MED API. This forwarding is accomplished by using the route specified in the `AI-MED_API_BASE_URL` environment variable. Therefore, a request made to `/AI-MED/api` in the Web browser is effectively the same as making a request to `AI-MED_API_BASE_URL` in the backend. For instance, a request to `/AI-MED/api/tags` in the WebUI is equivalent to `AI-MED_API_BASE_URL/tags` in the backend.

- **Security Benefits**: This design prevents direct exposure of the AID-MED API to the frontend, safeguarding against potential CORS (Cross-Origin Resource Sharing) issues and unauthorized access. Requiring authentication to access the AI-MED API further enhances this security layer.

## Ayonix AI-MED: Server Connection Error

If you're experiencing connection issues, it’s often due to the Webpage container not being able to reach the AI-MED server at 127.0.0.1:11434 inside the container . Use the `--network=host` flag in your command line to resolve this. Note that the port changes from 3000 to 8080, resulting in the link: `http://localhost:8080`.

### General Connection Errors

**Ensure AI-MED Version is Up-to-Date**: Always start by checking that you have the latest version of AI-MED. Visit Ayonix.com for the latest updates.

**Troubleshooting Steps**:

1. **Verify AI-MED URL Format**:
   - When running the AI-MED container, ensure the `AI-MED_API_BASE_URL` is correctly set, including the `/api` suffix. (e.g., `http://192.168.1.1:11434/api` for different host setups).
   - In the Ayonix AI-MED web, navigate to "Settings" > "General".
   - Confirm that the AI-MED Server URL is correctly set to `[AI-MED URL]/api` (e.g., `http://localhost:11434/api`), including the `/api` suffix.

By following these enhanced troubleshooting steps, connection issues should be effectively resolved. For further assistance or queries, feel free to reach out to us at aimed@ayonix.com.
