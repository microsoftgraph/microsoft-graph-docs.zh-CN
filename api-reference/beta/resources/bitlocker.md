---
title: bitlocker 类型
description: BitLocker 资源
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3ad8a05e82cd3f300bedf034fe18f67ce3359f16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038864"
---
# <a name="bitlocker-resource-type"></a><span data-ttu-id="e1045-103">bitlocker 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1045-103">bitlocker resource type</span></span>

<span data-ttu-id="e1045-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1045-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1045-105">存储的 BitLocker 密钥的父资源，其中包含包含实际恢复密钥的 **bitlockerRecoveryKey** 导航属性。</span><span class="sxs-lookup"><span data-stu-id="e1045-105">The parent resource for a stored BitLocker key with the navigation property **bitlockerRecoveryKey** which contains the actual recovery key.</span></span>

## <a name="methods"></a><span data-ttu-id="e1045-106">方法</span><span class="sxs-lookup"><span data-stu-id="e1045-106">Methods</span></span>
|<span data-ttu-id="e1045-107">方法</span><span class="sxs-lookup"><span data-stu-id="e1045-107">Method</span></span>|<span data-ttu-id="e1045-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e1045-108">Return type</span></span>|<span data-ttu-id="e1045-109">说明</span><span class="sxs-lookup"><span data-stu-id="e1045-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e1045-110">列出 recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="e1045-110">List recoveryKeys</span></span>](../api/bitlocker-list-recoverykeys.md)|<span data-ttu-id="e1045-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1045-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span>|<span data-ttu-id="e1045-112">获取 bitlockerRecoveryKey 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="e1045-112">Get a list of the bitlockerRecoveryKey objects and their properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1045-113">属性</span><span class="sxs-lookup"><span data-stu-id="e1045-113">Properties</span></span>
<span data-ttu-id="e1045-114">无。</span><span class="sxs-lookup"><span data-stu-id="e1045-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="e1045-115">关系</span><span class="sxs-lookup"><span data-stu-id="e1045-115">Relationships</span></span>
| <span data-ttu-id="e1045-116">关系</span><span class="sxs-lookup"><span data-stu-id="e1045-116">Relationship</span></span> | <span data-ttu-id="e1045-117">类型</span><span class="sxs-lookup"><span data-stu-id="e1045-117">Type</span></span> | <span data-ttu-id="e1045-118">说明</span><span class="sxs-lookup"><span data-stu-id="e1045-118">Description</span></span> |
|--|--|--|
| <span data-ttu-id="e1045-119">recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="e1045-119">recoveryKeys</span></span> | <span data-ttu-id="e1045-120">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1045-120">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span> | <span data-ttu-id="e1045-121">与 bitlocker 实体关联的恢复密钥。</span><span class="sxs-lookup"><span data-stu-id="e1045-121">The recovery keys associated with the bitlocker entity.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e1045-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1045-122">JSON representation</span></span>
<span data-ttu-id="e1045-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1045-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitlocker",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitlocker"
}
```

