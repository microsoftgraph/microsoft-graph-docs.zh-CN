---
title: educationOnPremisesInfo 资源类型
description: 用于将本地 Active Directory 用户帐户与 Azure AD 用户对象相关联的其他信息。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c147755aea584674e17f2de913e039b7d3e0cf82
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764741"
---
# <a name="educationonpremisesinfo-resource-type"></a><span data-ttu-id="82d58-103">educationOnPremisesInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="82d58-103">educationOnPremisesInfo resource type</span></span>

<span data-ttu-id="82d58-104">用于将本地 Active Directory 用户帐户与 Azure AD 用户对象相关联的其他信息。</span><span class="sxs-lookup"><span data-stu-id="82d58-104">Additional information used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span>

## <a name="properties"></a><span data-ttu-id="82d58-105">属性</span><span class="sxs-lookup"><span data-stu-id="82d58-105">Properties</span></span>

| <span data-ttu-id="82d58-106">属性</span><span class="sxs-lookup"><span data-stu-id="82d58-106">Property</span></span>    | <span data-ttu-id="82d58-107">类型</span><span class="sxs-lookup"><span data-stu-id="82d58-107">Type</span></span>   | <span data-ttu-id="82d58-108">说明</span><span class="sxs-lookup"><span data-stu-id="82d58-108">Description</span></span>                                               |
| :---------- | :----- | :-------------------------------------------------------- |
| <span data-ttu-id="82d58-109">immutableId</span><span class="sxs-lookup"><span data-stu-id="82d58-109">immutableId</span></span> | <span data-ttu-id="82d58-110">String</span><span class="sxs-lookup"><span data-stu-id="82d58-110">String</span></span> | <span data-ttu-id="82d58-111">Active Directory 中的 user 对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="82d58-111">Unique identifier for the user object in Active Directory.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="82d58-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82d58-112">JSON representation</span></span>

<span data-ttu-id="82d58-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82d58-113">The following is a JSON representation of the resource.</span></span>

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
