---
title: iosVppEBook 资源类型
description: 包含 iOS Vpp eBook的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8451018acf3405efb6176f33f5604ce630ca1d71
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730740"
---
# <a name="iosvppebook-resource-type"></a>iosVppEBook 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
|id|字符串|实体的键。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|displayName|String|电子图书的名称。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|说明|String|说明。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|publisher|String|发布者。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|publishedDateTime|DateTimeOffset|电子图书的发布日期和时间。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|书籍封面。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|createdDateTime|DateTimeOffset|电子图书文件的创建日期和时间。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改电子书的日期和时间。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|informationUrl|String|详细信息 URL。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
|privacyInformationUrl|String|隐私声明 URL。 继承自 [managedEBook](../resources/intune-books-managedebook.md)|
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





