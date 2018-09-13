# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation 资源类型

包含安全产品/服务提供商、提供程序和次级提供程序相关的详细信息（例如，vendor=Microsoft；provider=Windows Defender ATP；subProvider=AppLocker）。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|provider *|字符串|特定提供程序 （产品/服务 — 非供应商公司）；例如，WindowsDefenderATP。|
|providerVersion|字符串|生成提示的提供程序或次级提供程序（如果存在）的版本。|
|subProvider|字符串|特定次级提供程序（聚合提供程序之下）；例如，WindowsDefenderATP.SmartScreen。|
|vendor *|字符串|提示的供应商 (例如，Microsoft、Dell、FireEye) 的名称。|
（\* 表示必填字段。）

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
