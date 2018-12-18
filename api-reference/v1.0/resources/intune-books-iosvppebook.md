---
title: iosVppEBook 资源类型
description: 包含 iOS Vpp eBook的属性的类。
author: tfitzmac
ms.openlocfilehash: a54c3a846be339dd1b7dcb98169e249122899d84
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362088"
---
# <a name="iosvppebook-resource-type"></a>iosVppEBook 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含 iOS Vpp eBook的属性的类。

继承自 [managedEBook](../resources/intune-books-managedebook.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List iosVppEBooks](../api/intune-books-iosvppebook-list.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md) 集合|列出 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性和关系。|
|[Get iosVppEBook](../api/intune-books-iosvppebook-get.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|读取 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性和关系。|
|[Create iosVppEBook](../api/intune-books-iosvppebook-create.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|创建新的 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。|
|[Delete iosVppEBook](../api/intune-books-iosvppebook-delete.md)|无|删除 [iosVppEBook](../resources/intune-books-iosvppebook.md)。|
|[Update iosVppEBook](../api/intune-books-iosvppebook-update.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|更新 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|displayName|String|电子书的名称。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|description|String|说明。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|publisher|String|发布者。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|publishedDateTime|DateTimeOffset|电子书的发布日期和时间。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|书籍封面。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|createdDateTime|DateTimeOffset|电子书文件的创建日期和时间。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改电子书的日期和时间。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|informationUrl|String|详细信息 Url。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|privacyInformationUrl|String|隐私声明 Url。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|vppTokenId|Guid|Vpp 令牌 ID。|
|appleId|String|与 Vpp 令牌关联的 Apple ID。|
|vppOrganizationName|String|Vpp 令牌的组织名称。|
|genres|String 集合|流派。|
|language|String|语言。|
|seller|String|经销商。|
|totalLicenseCount|Int32|许可证总数。|
|usedLicenseCount|Int32|使用的许可证数。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合|此电子书的作业列表。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|installSummary|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|移动应用安装摘要。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|deviceStates|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合|此电子书的安装状态列表。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|userStateSummary|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合|此电子书的安装状态列表。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String",
  "vppTokenId": "Guid",
  "appleId": "String",
  "vppOrganizationName": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "seller": "String",
  "totalLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```



