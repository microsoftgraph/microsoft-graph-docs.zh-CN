---
title: userRegistrationCount 资源类型
description: 表示租户中用户的注册计数和状态。
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 5aa86a0b490ddb2cd68a504f5a4879f922fa0cf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057821"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="950eb-103">userRegistrationCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="950eb-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="950eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="950eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="950eb-105">表示租户中用户的注册计数和状态。</span><span class="sxs-lookup"><span data-stu-id="950eb-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="950eb-106">属性</span><span class="sxs-lookup"><span data-stu-id="950eb-106">Properties</span></span>

| <span data-ttu-id="950eb-107">属性</span><span class="sxs-lookup"><span data-stu-id="950eb-107">Property</span></span>     | <span data-ttu-id="950eb-108">类型</span><span class="sxs-lookup"><span data-stu-id="950eb-108">Type</span></span>        | <span data-ttu-id="950eb-109">说明</span><span class="sxs-lookup"><span data-stu-id="950eb-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="950eb-110">registrationCount</span><span class="sxs-lookup"><span data-stu-id="950eb-110">registrationCount</span></span> | <span data-ttu-id="950eb-111">Int64</span><span class="sxs-lookup"><span data-stu-id="950eb-111">Int64</span></span> | <span data-ttu-id="950eb-112">为你的租户提供注册计数。</span><span class="sxs-lookup"><span data-stu-id="950eb-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="950eb-113">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="950eb-113">registrationStatus</span></span> | <span data-ttu-id="950eb-114">String</span><span class="sxs-lookup"><span data-stu-id="950eb-114">String</span></span> | <span data-ttu-id="950eb-115">表示用户注册的状态。</span><span class="sxs-lookup"><span data-stu-id="950eb-115">Represents the status of user registration.</span></span> <span data-ttu-id="950eb-116">可能的值是： `registered` 、 `enabled` 、 `capable` 和 `mfaRegistered` 。</span><span class="sxs-lookup"><span data-stu-id="950eb-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="950eb-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="950eb-117">JSON representation</span></span>

<span data-ttu-id="950eb-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="950eb-118">The following is a JSON representation of the resource.</span></span>

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

