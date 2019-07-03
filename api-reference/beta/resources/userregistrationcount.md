---
title: userRegistrationCount 资源类型
description: 表示租户中用户的注册计数和状态。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 43f151864f7ca996602e7bd2fc42f3fa4ba743d1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480139"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="f94af-103">userRegistrationCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="f94af-103">userRegistrationCount resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f94af-104">表示租户中用户的注册计数和状态。</span><span class="sxs-lookup"><span data-stu-id="f94af-104">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="f94af-105">属性</span><span class="sxs-lookup"><span data-stu-id="f94af-105">Properties</span></span>

| <span data-ttu-id="f94af-106">属性</span><span class="sxs-lookup"><span data-stu-id="f94af-106">Property</span></span>     | <span data-ttu-id="f94af-107">类型</span><span class="sxs-lookup"><span data-stu-id="f94af-107">Type</span></span>        | <span data-ttu-id="f94af-108">说明</span><span class="sxs-lookup"><span data-stu-id="f94af-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f94af-109">registrationCount</span><span class="sxs-lookup"><span data-stu-id="f94af-109">registrationCount</span></span> | <span data-ttu-id="f94af-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f94af-110">Int64</span></span> | <span data-ttu-id="f94af-111">为你的租户提供注册计数。</span><span class="sxs-lookup"><span data-stu-id="f94af-111">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="f94af-112">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="f94af-112">registrationStatus</span></span> | <span data-ttu-id="f94af-113">String</span><span class="sxs-lookup"><span data-stu-id="f94af-113">String</span></span> | <span data-ttu-id="f94af-114">表示用户注册的状态。</span><span class="sxs-lookup"><span data-stu-id="f94af-114">Represents the status of user registration.</span></span> <span data-ttu-id="f94af-115">可能的值是`registered`: `enabled`、 `capable`、和`mfaRegistered`。</span><span class="sxs-lookup"><span data-stu-id="f94af-115">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f94af-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f94af-116">JSON representation</span></span>

<span data-ttu-id="f94af-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f94af-117">The following is a JSON representation of the resource.</span></span>

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