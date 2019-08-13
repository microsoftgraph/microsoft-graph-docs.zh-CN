---
title: macOSKernelExtension 资源类型
description: 表示特定的 macOS 内核扩展。 MacOS 内核扩展可以通过其团队标识符加上其捆绑包标识符进行描述。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fbf12bd16bdf606010bc9b6518c8241fe28eb765
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321930"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="43676-104">macOSKernelExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="43676-104">macOSKernelExtension resource type</span></span>

> <span data-ttu-id="43676-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43676-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43676-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43676-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43676-107">表示特定的 macOS 内核扩展。</span><span class="sxs-lookup"><span data-stu-id="43676-107">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="43676-108">MacOS 内核扩展可以通过其团队标识符加上其捆绑包标识符进行描述。</span><span class="sxs-lookup"><span data-stu-id="43676-108">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="43676-109">属性</span><span class="sxs-lookup"><span data-stu-id="43676-109">Properties</span></span>
|<span data-ttu-id="43676-110">属性</span><span class="sxs-lookup"><span data-stu-id="43676-110">Property</span></span>|<span data-ttu-id="43676-111">类型</span><span class="sxs-lookup"><span data-stu-id="43676-111">Type</span></span>|<span data-ttu-id="43676-112">说明</span><span class="sxs-lookup"><span data-stu-id="43676-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43676-113">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="43676-113">teamIdentifier</span></span>|<span data-ttu-id="43676-114">String</span><span class="sxs-lookup"><span data-stu-id="43676-114">String</span></span>|<span data-ttu-id="43676-115">用于对内核扩展进行签名的团队标识符。</span><span class="sxs-lookup"><span data-stu-id="43676-115">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="43676-116">bundleId</span><span class="sxs-lookup"><span data-stu-id="43676-116">bundleId</span></span>|<span data-ttu-id="43676-117">String</span><span class="sxs-lookup"><span data-stu-id="43676-117">String</span></span>|<span data-ttu-id="43676-118">内核扩展的捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="43676-118">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43676-119">关系</span><span class="sxs-lookup"><span data-stu-id="43676-119">Relationships</span></span>
<span data-ttu-id="43676-120">无</span><span class="sxs-lookup"><span data-stu-id="43676-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43676-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43676-121">JSON Representation</span></span>
<span data-ttu-id="43676-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43676-122">Here is a JSON representation of the resource.</span></span>
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



