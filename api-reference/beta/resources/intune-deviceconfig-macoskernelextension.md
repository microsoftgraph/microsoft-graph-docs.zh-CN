---
title: macOSKernelExtension 资源类型
description: 表示特定的 macOS 内核扩展。 MacOS 内核扩展可以通过其团队标识符加上其捆绑包标识符进行描述。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 457d13b2f3f78b52457afd7c30bf3b0e36ca4e92
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447050"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="36157-104">macOSKernelExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="36157-104">macOSKernelExtension resource type</span></span>

<span data-ttu-id="36157-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36157-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36157-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="36157-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36157-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36157-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36157-108">表示特定的 macOS 内核扩展。</span><span class="sxs-lookup"><span data-stu-id="36157-108">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="36157-109">MacOS 内核扩展可以通过其团队标识符加上其捆绑包标识符进行描述。</span><span class="sxs-lookup"><span data-stu-id="36157-109">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="36157-110">属性</span><span class="sxs-lookup"><span data-stu-id="36157-110">Properties</span></span>
|<span data-ttu-id="36157-111">属性</span><span class="sxs-lookup"><span data-stu-id="36157-111">Property</span></span>|<span data-ttu-id="36157-112">类型</span><span class="sxs-lookup"><span data-stu-id="36157-112">Type</span></span>|<span data-ttu-id="36157-113">说明</span><span class="sxs-lookup"><span data-stu-id="36157-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36157-114">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="36157-114">teamIdentifier</span></span>|<span data-ttu-id="36157-115">String</span><span class="sxs-lookup"><span data-stu-id="36157-115">String</span></span>|<span data-ttu-id="36157-116">用于对内核扩展进行签名的团队标识符。</span><span class="sxs-lookup"><span data-stu-id="36157-116">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="36157-117">bundleId</span><span class="sxs-lookup"><span data-stu-id="36157-117">bundleId</span></span>|<span data-ttu-id="36157-118">String</span><span class="sxs-lookup"><span data-stu-id="36157-118">String</span></span>|<span data-ttu-id="36157-119">内核扩展的捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="36157-119">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36157-120">关系</span><span class="sxs-lookup"><span data-stu-id="36157-120">Relationships</span></span>
<span data-ttu-id="36157-121">无</span><span class="sxs-lookup"><span data-stu-id="36157-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36157-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36157-122">JSON Representation</span></span>
<span data-ttu-id="36157-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36157-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKernelExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKernelExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```



