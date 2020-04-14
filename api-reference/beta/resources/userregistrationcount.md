---
title: userRegistrationCount 资源类型
description: 表示租户中用户的注册计数和状态。
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: e322f073655ffaa975464d666a365410138f6e51
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384978"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="7b04b-103">userRegistrationCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b04b-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="7b04b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b04b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b04b-105">表示租户中用户的注册计数和状态。</span><span class="sxs-lookup"><span data-stu-id="7b04b-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="7b04b-106">属性</span><span class="sxs-lookup"><span data-stu-id="7b04b-106">Properties</span></span>

| <span data-ttu-id="7b04b-107">属性</span><span class="sxs-lookup"><span data-stu-id="7b04b-107">Property</span></span>     | <span data-ttu-id="7b04b-108">类型</span><span class="sxs-lookup"><span data-stu-id="7b04b-108">Type</span></span>        | <span data-ttu-id="7b04b-109">说明</span><span class="sxs-lookup"><span data-stu-id="7b04b-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7b04b-110">registrationCount</span><span class="sxs-lookup"><span data-stu-id="7b04b-110">registrationCount</span></span> | <span data-ttu-id="7b04b-111">Int64</span><span class="sxs-lookup"><span data-stu-id="7b04b-111">Int64</span></span> | <span data-ttu-id="7b04b-112">为你的租户提供注册计数。</span><span class="sxs-lookup"><span data-stu-id="7b04b-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="7b04b-113">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="7b04b-113">registrationStatus</span></span> | <span data-ttu-id="7b04b-114">字符串</span><span class="sxs-lookup"><span data-stu-id="7b04b-114">String</span></span> | <span data-ttu-id="7b04b-115">表示用户注册的状态。</span><span class="sxs-lookup"><span data-stu-id="7b04b-115">Represents the status of user registration.</span></span> <span data-ttu-id="7b04b-116">可能的值是`registered`： `enabled`、 `capable`、和`mfaRegistered`。</span><span class="sxs-lookup"><span data-stu-id="7b04b-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b04b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b04b-117">JSON representation</span></span>

<span data-ttu-id="7b04b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b04b-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userRegistrationCount",
  "baseType": null
}-->

```json
{ 
  "registrationStatus":"String", 
  "registrationCount": 23423
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->