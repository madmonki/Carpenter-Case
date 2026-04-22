# Carpenter-Case

This repository contains a multiplayer system prototype developed with Unreal Engine 5.7,
built on a Server-Authoritative architecture. The core development focus is on secure network communication,
optimized rendering mechanics, and fluid user interface interactions.

##  Technical Details & Development Approach

* **Networking & Multiplayer:** 
  * Fully Server-Authoritative architecture with Dedicated Server compatibility.
  * Server-side managed, cheat-proof custom Spawn algorithm that generates no network traffic (Non-Replicated State).
  * Optimized RPC and RepNotify (Multicast) integrations to preserve bandwidth.

* **Gameplay Logic:**
  * Timer and State Lock based Cooldown systems designed to prevent input spamming.
  * Dynamic overlap and collision logic with reduced error margins for order and delivery (Pickup/Drop) loops.

* **User Interface (UMG/UI):**
  * Reactive UI components utilizing dynamic state binding.
  * Performant state animations (e.g., slide-in/fade-out effects for income/expense) created using UMG Timelines and Slate architecture.

