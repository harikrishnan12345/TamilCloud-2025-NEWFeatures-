The “Skip OS Shutdown” option is basically a fast-track stop/terminate.

Without it (default): AWS sends the shutdown signal → OS takes time to gracefully stop services → then the instance powers off.

With Skip OS Shutdown: AWS immediately cuts power → the instance stops/terminates much faster (like holding down the power button on a laptop).

So yes — it speeds up termination/stop, but at the cost of skipping the OS’s cleanup phase (risking data loss or corruption).