---
title: userRegistrationCount 资源类型
description: 表示租户中用户的注册计数和状态。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5cdcdb4cfd56c0828cfeb7e71defe4c7459e3133
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132949"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="03aad-103">userRegistrationCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="03aad-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="03aad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03aad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03aad-105">表示租户中用户的注册计数和状态。</span><span class="sxs-lookup"><span data-stu-id="03aad-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="03aad-106">属性</span><span class="sxs-lookup"><span data-stu-id="03aad-106">Properties</span></span>

| <span data-ttu-id="03aad-107">属性</span><span class="sxs-lookup"><span data-stu-id="03aad-107">Property</span></span>     | <span data-ttu-id="03aad-108">类型</span><span class="sxs-lookup"><span data-stu-id="03aad-108">Type</span></span>        | <span data-ttu-id="03aad-109">说明</span><span class="sxs-lookup"><span data-stu-id="03aad-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="03aad-110">registrationCount</span><span class="sxs-lookup"><span data-stu-id="03aad-110">registrationCount</span></span> | <span data-ttu-id="03aad-111">Int64</span><span class="sxs-lookup"><span data-stu-id="03aad-111">Int64</span></span> | <span data-ttu-id="03aad-112">提供租户的注册计数。</span><span class="sxs-lookup"><span data-stu-id="03aad-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="03aad-113">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="03aad-113">registrationStatus</span></span> | <span data-ttu-id="03aad-114">字符串</span><span class="sxs-lookup"><span data-stu-id="03aad-114">String</span></span> | <span data-ttu-id="03aad-115">表示用户注册的状态。</span><span class="sxs-lookup"><span data-stu-id="03aad-115">Represents the status of user registration.</span></span> <span data-ttu-id="03aad-116">可能的值是： `registered` 、 `enabled` 和 `capable` `mfaRegistered` 。</span><span class="sxs-lookup"><span data-stu-id="03aad-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="03aad-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03aad-117">JSON representation</span></span>

<span data-ttu-id="03aad-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03aad-118">The following is a JSON representation of the resource.</span></span>

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

