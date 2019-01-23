---
title: dataSharingConsent 资源类型
description: 数据共享许可信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bf77a252c323ce83c2dcda44ac294161a4fd4747
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425692"
---
# <a name="datasharingconsent-resource-type"></a>dataSharingConsent 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
|id|String|数据共享同意 Id|
|serviceDisplayName|String|服务工作流的显示名称|
|termsUrl|String|数据共享同意 TermsUrl|
|granted|Boolean|数据共享同意向其授予的状态|
|grantDateTime|DateTimeOffset|此帐户授予时间同意|
|grantedByUpn|String|用户授予许可，为此帐户的 Upn|
|grantedByUserId|String|授予许可，为此帐户的用户的用户 Id|

## <a name="relationships"></a>关系
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




