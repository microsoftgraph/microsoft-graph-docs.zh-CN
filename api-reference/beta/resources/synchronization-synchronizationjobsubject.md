---
title: synchronizationJobSubject 资源类型
description: 表示在按需预配期间预配的对象。
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 2e6a0bea0f3e035bc5b0aef81a20b4a9dc480836
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441676"
---
# <a name="synchronizationjobsubject-resource-type"></a>synchronizationJobSubject 资源类型

命名空间：microsoft.graph

表示在按需预配期间预配的对象。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|links|[synchronizationLinkedObjects](../resources/synchronizationlinkedobjects.md)|要预配的主体。|
|objectId|String|要向其应用 **synchronizationJob** 的对象的标识符。 可以是下列类型之一： <li>用于从 Active Directory 同步到 Azure AD 的 **onPremisesDistinguishedName** 。</li><li>用于从 Azure AD 同步到第三方的用户 ID。</li><li>要从 Workday 同步到 Active Directory 或 Azure AD 的 Workday 辅助角色的辅助角色 ID。</li>|
|objectTypeName|String|要向其应用 **synchronizationJob** 的对象的类型。 可以是下列类型之一： <li>`user` 用于在 Active Directory 和 Azure AD 之间同步。</li><li>`User` 用于在 Azure AD 和第三方应用程序之间同步用户。 </li><li>`Worker` 用于在 Workday 和 Active Directory 或 Azure AD 之间同步用户。</li><li>`Group` 用于在 Azure AD 和第三方应用程序之间同步组。 </li>|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobSubject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobSubject",
  "objectId": "String",
  "objectTypeName": "String",
  "links": {
    "@odata.type": "microsoft.graph.synchronizationLinkedObjects"
  }
}
```


