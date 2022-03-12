---
title: 协议资源类型
description: 表示租户的可自定义使用条款协议，该协议是使用 Azure Active Directory (Azure AD) 。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: b58bd212dd4960bdb5e19967f3b43237caf384ce
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451436"
---
# <a name="agreement-resource-type"></a>协议资源类型

命名空间：microsoft.graph

表示租户的可自定义使用条款协议，该协议是使用 Azure Active Directory (Azure AD) 。 您可以使用以下方法根据你的方案创建和管理Azure Active Directory[使用条款](/azure/active-directory/conditional-access/terms-of-use)"功能。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/termsofusecontainer-list-agreements.md) | [协议](agreement.md) 集合 | 获取协议对象集合。 |
| [Create](../api/termsofusecontainer-post-agreements.md) | [协议](agreement.md) | 通过发布到协议集合创建新协议。 |
| [Get](../api/agreement-get.md) | [协议](agreement.md) | 读取协议对象的属性和关系。 |
| [更新](../api/agreement-update.md) | 无 | 更新协议对象。 |
| [删除](../api/agreement-delete.md) | 无 | 删除协议对象。 |
|[列出接受](../api/agreement-list-acceptances.md)|[agreementAcceptance](../resources/agreementacceptance.md) 集合|获取有关特定协议的接受记录的详细信息。|
|[List agreementAcceptances](../api/user-list-agreementacceptances.md)|[agreementAcceptance](../resources/agreementacceptance.md) 集合|获取已登录用户的协议接受。|
|[获取 agreementFile](../api/agreementfile-get.md)|[agreementFile](../resources/agreementfile.md) 集合|检索协议的默认文件的详细信息，包括语言和版本信息。|
|[列出文件](../api/agreement-list-files.md)|[agreementFileLocalization](../resources/agreementfilelocalization.md) 集合|检索与协议相关的所有本地化文件。|
|[创建 agreementFileLocalization](../api/agreement-post-files.md)|[agreementFileLocalization](../resources/agreementfilelocalization.md)|创建新的本地化协议文件。|

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|字符串|协议的显示名称。 The 显示名称 is used for internal tracking of the agreement but is not shown to end users who view the agreement. 支持 `$filter`（`eq`）。|
|id|字符串| 协议的标识符。 只读。 支持 `$filter`（`eq`）。|
|isPerDeviceAcceptanceRequired|布尔值|指示最终用户是否需要在从其访问它的每个设备上接受此协议。 如果最终用户尚未注册设备，Azure AD注册设备。 支持 `$filter`（`eq`）。|
|isViewingBeforeAcceptanceRequired|布尔值|指示用户是否必须扩展协议才能接受。 支持 `$filter`（`eq`）。|
|termsExpiration|[termsExpiration](termsexpiration.md)| 所有用户的过期日程安排和协议频率。 支持 `$filter`（`eq`）。|
|userReacceptRequiredFrequency|期限|用户必须重新接受使用条款的持续时间。 该值以 ISO 8601 格式表示，持续时间为。 支持 `$filter`（`eq`）。|


## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|接受|[agreementAcceptance](agreementacceptance.md) 集合|只读。 有关接受本协议的信息。|
|file|[agreementFile](agreementfile.md) | 链接到本协议的默认 PDF。|
|files|[agreementFileLocalization](agreementfilelocalization.md) 集合| 链接到本协议的 PDF。 此属性正在被弃用。 请  **改为使用 file** 属性。 支持 `$expand`。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.agreement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.agreement",
  "id": "String (identifier)",
  "displayName": "String",
  "termsExpiration": {
    "@odata.type": "microsoft.graph.termsExpiration"
  },
  "userReacceptRequiredFrequency": "String (duration)",
  "isViewingBeforeAcceptanceRequired": "Boolean",
  "isPerDeviceAcceptanceRequired": "Boolean"
}
```
