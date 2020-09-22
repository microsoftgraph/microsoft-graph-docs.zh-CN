---
title: educationOnPremisesInfo 资源类型
description: 用于将本地 Active Directory 用户帐户与 Azure AD 用户对象相关联的其他信息。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ff575398f3829c5d2adbe92799f5b9dca953aa4e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998822"
---
# <a name="educationonpremisesinfo-resource-type"></a><span data-ttu-id="96d2d-103">educationOnPremisesInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="96d2d-103">educationOnPremisesInfo resource type</span></span>

<span data-ttu-id="96d2d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96d2d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96d2d-105">用于将本地 Active Directory 用户帐户与 Azure AD 用户对象相关联的其他信息。</span><span class="sxs-lookup"><span data-stu-id="96d2d-105">Additional information used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span>

## <a name="properties"></a><span data-ttu-id="96d2d-106">属性</span><span class="sxs-lookup"><span data-stu-id="96d2d-106">Properties</span></span>

| <span data-ttu-id="96d2d-107">属性</span><span class="sxs-lookup"><span data-stu-id="96d2d-107">Property</span></span>    | <span data-ttu-id="96d2d-108">类型</span><span class="sxs-lookup"><span data-stu-id="96d2d-108">Type</span></span>   | <span data-ttu-id="96d2d-109">说明</span><span class="sxs-lookup"><span data-stu-id="96d2d-109">Description</span></span>                                               |
| :---------- | :----- | :-------------------------------------------------------- |
| <span data-ttu-id="96d2d-110">immutableId</span><span class="sxs-lookup"><span data-stu-id="96d2d-110">immutableId</span></span> | <span data-ttu-id="96d2d-111">String</span><span class="sxs-lookup"><span data-stu-id="96d2d-111">String</span></span> | <span data-ttu-id="96d2d-112">Active Directory 中的 user 对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="96d2d-112">Unique identifier for the user object in Active Directory.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="96d2d-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96d2d-113">JSON representation</span></span>

<span data-ttu-id="96d2d-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96d2d-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}-->

```json
{
  "immutableId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOnPremisesInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


