---
title: dataSharingConsent 资源类型
description: 数据共享同意信息。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 92c012f994c3e5aa3630f05632d48df764a432d7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057325"
---
# <a name="datasharingconsent-resource-type"></a>dataSharingConsent 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

数据共享同意信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 dataSharingConsents](../api/intune-devices-datasharingconsent-list.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) 集合|列出 [dataSharingConsent 对象的属性和](../resources/intune-devices-datasharingconsent.md) 关系。|
|[获取 dataSharingConsent](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|读取 [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) 对象的属性和关系。|
|[创建 dataSharingConsent](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|创建新的 [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) 对象。|
|[删除 dataSharingConsent](../api/intune-devices-datasharingconsent-delete.md)|无|删除 [dataSharingConsent](../resources/intune-devices-datasharingconsent.md)。|
|[更新 dataSharingConsent](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|更新 [dataSharingConsent 对象](../resources/intune-devices-datasharingconsent.md) 的属性。|
|[consentToDataSharing 操作](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|数据共享许可 ID|
|serviceDisplayName|String|服务显示名称流|
|termsUrl|String|数据共享同意的 TermsUrl|
|granted|Boolean|数据共享同意的授予状态|
|grantDateTime|DateTimeOffset|为此帐户授予许可的时间|
|grantedByUpn|String|授予此帐户同意的用户的 Upn|
|grantedByUserId|String|授予此帐户同意的用户的 UserId|

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



