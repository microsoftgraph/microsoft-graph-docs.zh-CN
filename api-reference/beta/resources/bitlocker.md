---
title: bitlocker 类型
description: BitLocker 资源
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3e714015b3834051371861880355360f02d12166
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761833"
---
# <a name="bitlocker-resource-type"></a><span data-ttu-id="a18e4-103">bitlocker 资源类型</span><span class="sxs-lookup"><span data-stu-id="a18e4-103">bitlocker resource type</span></span>

<span data-ttu-id="a18e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a18e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a18e4-105">包含实际恢复密钥的导航属性 **bitlockerRecoveryKey** 的已存储 BitLocker 密钥的父资源。</span><span class="sxs-lookup"><span data-stu-id="a18e4-105">The parent resource for a stored BitLocker key with the navigation property **bitlockerRecoveryKey** which contains the actual recovery key.</span></span>

## <a name="methods"></a><span data-ttu-id="a18e4-106">方法</span><span class="sxs-lookup"><span data-stu-id="a18e4-106">Methods</span></span>
|<span data-ttu-id="a18e4-107">方法</span><span class="sxs-lookup"><span data-stu-id="a18e4-107">Method</span></span>|<span data-ttu-id="a18e4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a18e4-108">Return type</span></span>|<span data-ttu-id="a18e4-109">说明</span><span class="sxs-lookup"><span data-stu-id="a18e4-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a18e4-110">列出 recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="a18e4-110">List recoveryKeys</span></span>](../api/bitlocker-list-recoverykeys.md)|<span data-ttu-id="a18e4-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a18e4-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span>|<span data-ttu-id="a18e4-112">获取 bitlockerRecoveryKey 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="a18e4-112">Get a list of the bitlockerRecoveryKey objects and their properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="a18e4-113">属性</span><span class="sxs-lookup"><span data-stu-id="a18e4-113">Properties</span></span>
<span data-ttu-id="a18e4-114">无。</span><span class="sxs-lookup"><span data-stu-id="a18e4-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="a18e4-115">关系</span><span class="sxs-lookup"><span data-stu-id="a18e4-115">Relationships</span></span>
| <span data-ttu-id="a18e4-116">关系</span><span class="sxs-lookup"><span data-stu-id="a18e4-116">Relationship</span></span> | <span data-ttu-id="a18e4-117">类型</span><span class="sxs-lookup"><span data-stu-id="a18e4-117">Type</span></span> | <span data-ttu-id="a18e4-118">说明</span><span class="sxs-lookup"><span data-stu-id="a18e4-118">Description</span></span> |
|--|--|--|
| <span data-ttu-id="a18e4-119">recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="a18e4-119">recoveryKeys</span></span> | <span data-ttu-id="a18e4-120">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a18e4-120">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span> | <span data-ttu-id="a18e4-121">与 bitlocker 实体关联的恢复密钥。</span><span class="sxs-lookup"><span data-stu-id="a18e4-121">The recovery keys associated with the bitlocker entity.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a18e4-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a18e4-122">JSON representation</span></span>
<span data-ttu-id="a18e4-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a18e4-123">The following is a JSON representation of the resource.</span></span>
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

