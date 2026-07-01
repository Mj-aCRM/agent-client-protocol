<a href="https://agentclientprotocol.com/" >
  <img alt="بروتوكول العميل-الوكيل" src="https://zed.dev/img/acp/banner-dark.webp">
</a>

# بروتوكول العميل-الوكيل (ACP)

بروتوكول العميل-الوكيل (ACP) يُوحِّد التواصل بين _محرِّرات الكود_ (برامج تفاعلية لعرض وتحرير الكود المصدري) و*وكلاء البرمجة* (برامج تستخدم الذكاء الاصطناعي التوليدي لتعديل الكود بشكل مستقل).

اعرف المزيد على [agentclientprotocol.com](https://agentclientprotocol.com/).

---

**[English](./README.md)** | **العربية**

---

## حزمة Rust والتعريفات

الحزمة الرئيسية لهذا المستودع هي [`agent-client-protocol-schema`](https://crates.io/crates/agent-client-protocol-schema). توفر نموذج بيانات Rust لرسائل بروتوكول ACP، بما في ذلك أنواع الطلب والاستجابة والإشعارات ومغلف JSON-RPC وأنواع إصدار البروتوكول.

إذا كنت تبني وكيلاً أو عميلاً بـ Rust، ابدأ بحزمة [`agent-client-protocol`](https://crates.io/crates/agent-client-protocol) ذات المستوى الأعلى.

ملفات JSON Schema المُولَّدة موجودة في [`schema/v1`](./schema/v1/) و[`schema/v2`](./schema/v2/).

## الإصدار

**إصدار بروتوكول ACP الحالي المستقر هو `1`.**

توافق الـ wire يُحدَّد بشكل منفصل عبر `protocolVersion` المُتبادَل أثناء `initialize`.

## التكاملات

- [المخطط (Schema)](./schema/v1/schema.json)
- [الوكلاء (Agents)](https://agentclientprotocol.com/overview/agents)
- [العملاء (Clients)](https://agentclientprotocol.com/overview/clients)
- المكتبات الرسمية:
  - **Kotlin**: [`acp-kotlin`](https://github.com/agentclientprotocol/kotlin-sdk)
  - **Java**: [`java-sdk`](https://github.com/agentclientprotocol/java-sdk)
  - **Python**: [`python-sdk`](https://github.com/agentclientprotocol/python-sdk)
  - **Rust**: [`agent-client-protocol`](https://crates.io/crates/agent-client-protocol)
  - **TypeScript**: [`@agentclientprotocol/sdk`](https://www.npmjs.com/package/@agentclientprotocol/sdk)
- [المكتبات المجتمعية](https://agentclientprotocol.com/libraries/community)

## المساهمة

ACP بروتوكول مُصمَّم للتبني الواسع عبر المنظومة البرمجية؛ نتبع عملية منظمة لضمان دراسة التغييرات جيدًا. اقرأ [دليل المساهمة](./CONTRIBUTING.md) للمزيد.

## الترخيص

هذا المشروع مرخص بموجب [رخصة Apache 2.0](./LICENSE).
