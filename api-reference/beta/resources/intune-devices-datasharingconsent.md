---
title: dataSharingConsent 资源类型
description: 数据共享许可信息。
author: tfitzmac
ms.openlocfilehash: 250ad388a5c619a6fd2753d172734145ea720776
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342932"
---
# <a name="datasharingconsent-resource-type"></a>dataSharingConsent 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

数据共享许可信息。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 dataSharingConsents](../api/intune-devices-datasharingconsent-list.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)集合|列出属性和[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象之间的关系。|
|[获取 dataSharingConsent](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|读取属性和[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的关系。|
|[创建 dataSharingConsent](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|创建新的[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象。|
|[删除 dataSharingConsent](../api/intune-devices-datasharingconsent-delete.md)|无|删除[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)。|
|[更新 dataSharingConsent](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|更新[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的属性。|
|[consentToDataSharing 操作](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|数据共享同意 Id|
|serviceDisplayName|字符串|服务工作流的显示名称|
|termsUrl|字符串|数据共享同意 TermsUrl|
|授予|Boolean|数据共享同意向其授予的状态|
|grantDateTime|DateTimeOffset|此帐户授予时间同意|
|grantedByUpn|字符串|用户授予许可，为此帐户的 Upn|
|grantedByUserId|字符串|授予许可，为此帐户的用户的用户 Id|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSharingConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": true,
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```





