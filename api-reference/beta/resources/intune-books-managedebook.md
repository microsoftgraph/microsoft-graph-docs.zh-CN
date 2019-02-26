---
title: managedEBook 资源类型
description: 包含托管电子书基属性的抽象类。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24a8619d92eee6c666b7126a84895b14e0404755
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156033"
---
# <a name="managedebook-resource-type"></a>managedEBook 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含托管电子书基属性的抽象类。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedEBooks](../api/intune-books-managedebook-list.md)|[managedEBook](../resources/intune-books-managedebook.md) 集合|列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。|
|[Get managedEBook](../api/intune-books-managedebook-get.md)|[managedEBook](../resources/intune-books-managedebook.md)|读取 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。|
|[assign 操作](../api/intune-books-managedebook-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|displayName|String|电子书的名称。|
|description|字符串|说明。|
|publisher|String|发布者。|
|publishedDateTime|DateTimeOffset|电子书的发布日期和时间。|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|书籍封面。|
|createdDateTime|DateTimeOffset|电子书文件的创建日期和时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改电子书的日期和时间。|
|informationUrl|String|详细信息 Url。|
|privacyInformationUrl|String|隐私声明 Url。|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|categories|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合|此电子书的类别列表。|
|assignments|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合|此电子书的分配列表。|
|installSummary|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|移动应用安装摘要。|
|deviceStates|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合|此电子书的安装状态列表。|
|userStateSummary|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合|此电子书的安装状态列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
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
  "privacyInformationUrl": "String"
}
```




