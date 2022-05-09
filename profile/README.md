# Sneller's TL/DR

Sneller is a cloud-native, serverless SQL engine designed specifically for JSON. With Sneller, you can run interactive SQL on large TB-sized datasets of deeply nested semi-structured JSON. Target use cases are event data pipelines such as Security, Observability, Ops, User Events and Sensor/IoT.

Sneller's performance derives from pervasive use of SIMD, specifically AVX-512 assembly in its 250+ core primitives. The main engine is capable of processing many lanes in parallel per core for very high processing throughputs. Combined with the fact that Sneller's main 'API' is SQL (with JSON output results), this greatly simplifies data processing pipelines.

Sneller is fully stateless and all state is stored exclusively on object storage. There are no other dependencies, such as meta-databases or key/value stores, to install, manage and maintain. This allows Sneller to scale very dynamically to adapt for varying query loads.
