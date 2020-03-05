---
title: userRegistrationCount 资源类型
description: 表示租户中用户的注册计数和状态。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 2b1a7d2c34ff21c8efd57b358864c4d218630594
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519517"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="91170-103">userRegistrationCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="91170-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="91170-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="91170-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91170-105">表示租户中用户的注册计数和状态。</span><span class="sxs-lookup"><span data-stu-id="91170-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="91170-106">属性</span><span class="sxs-lookup"><span data-stu-id="91170-106">Properties</span></span>

| <span data-ttu-id="91170-107">属性</span><span class="sxs-lookup"><span data-stu-id="91170-107">Property</span></span>     | <span data-ttu-id="91170-108">类型</span><span class="sxs-lookup"><span data-stu-id="91170-108">Type</span></span>        | <span data-ttu-id="91170-109">说明</span><span class="sxs-lookup"><span data-stu-id="91170-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="91170-110">registrationCount</span><span class="sxs-lookup"><span data-stu-id="91170-110">registrationCount</span></span> | <span data-ttu-id="91170-111">Int64</span><span class="sxs-lookup"><span data-stu-id="91170-111">Int64</span></span> | <span data-ttu-id="91170-112">为你的租户提供注册计数。</span><span class="sxs-lookup"><span data-stu-id="91170-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="91170-113">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="91170-113">registrationStatus</span></span> | <span data-ttu-id="91170-114">String</span><span class="sxs-lookup"><span data-stu-id="91170-114">String</span></span> | <span data-ttu-id="91170-115">表示用户注册的状态。</span><span class="sxs-lookup"><span data-stu-id="91170-115">Represents the status of user registration.</span></span> <span data-ttu-id="91170-116">可能的值是`registered`： `enabled`、 `capable`、和`mfaRegistered`。</span><span class="sxs-lookup"><span data-stu-id="91170-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="91170-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91170-117">JSON representation</span></span>

<span data-ttu-id="91170-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91170-118">The following is a JSON representation of the resource.</span></span>

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