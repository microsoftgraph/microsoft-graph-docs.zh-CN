---
title: synchronizationJobSubject 资源类型
description: 表示在按需预配期间预配的对象。
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: d9c19bc431ce152bb3b15f97822ee86071c314d8
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061116"
---
# <a name="synchronizationjobsubject-resource-type"></a>synchronizationJobSubject 资源类型

命名空间：microsoft.graph

表示在按需预配期间预配的对象。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|objectId|String|要向其应用 **synchronizationJob** 的对象的标识符。 可以是下列类型之一： <li>一个 **onPremisesDistinguishedName**，用于从 Active Directory 同步到Azure AD。</li><li>用于从Azure AD同步到第三方的用户 ID。</li><li>从 Workday 同步到 Active Directory 或 Azure AD 的 Workday 辅助角色的工作器 ID。</li>|
|objectTypeName|字符串|要向其应用 **synchronizationJob** 的对象的类型。 可以是下列类型之一： <li>`user`用于从 Active Directory 同步到Azure AD。</li><li>`User`用于从Azure AD同步到第三方应用程序。 </li><li>`Worker`从 Workday 同步到 Active Directory 或 Azure AD。</li>|

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
  "objectTypeName": "String"
}
```


