---
title: crossTenantAccessPolicyTarget 资源类型
description: 定义如何面向跨租户访问策略设置。 设置可以针对特定用户、组或应用程序。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 19f58264312d8f1b519d9de9b6f66365c29f0def
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604627"
---
# <a name="crosstenantaccesspolicytarget-resource-type"></a>crossTenantAccessPolicyTarget 资源类型

命名空间：microsoft.graph

定义如何面向跨租户访问策略设置。 设置可以针对特定用户、组或应用程序。 还可以使用关键字来定位特定组或应用程序。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| target | String | 用户、组或应用程序的唯一标识符;以下关键字之一：和`AllApplications`;`AllUsers`或者对于应用程序的目标，可以使用[保留值](#reserved-values-for-targets-that-are-applications)。 |
| targetType | crossTenantAccessPolicyTargetType | 要面向的资源类型。 可能的值包括 `user`、`group`、`application`、`unknownFutureValue`。 |

### <a name="reserved-values-for-targets-that-are-applications"></a>应用程序目标的保留值

设置应用程序目标时，还可以使用以下保留值：

| 符号 | 说明 |
|:---|:---|
| AllMicrosoftApps | 引用任何 [Microsoft 云应用程序](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps#microsoft-cloud-applications)。 |
| Office365 | 包括作为 [Office365](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps#office-365) 套件的一部分提到的应用程序。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyTarget"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyTarget",
  "target": "String",
  "targetType": "microsoft.graph.crossTenantAccessPolicyTargetType"
}
```
