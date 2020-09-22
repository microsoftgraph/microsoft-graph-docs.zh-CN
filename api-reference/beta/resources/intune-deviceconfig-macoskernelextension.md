---
title: macOSKernelExtension 资源类型
description: 表示特定的 macOS 内核扩展。 MacOS 内核扩展可以通过其团队标识符加上其捆绑包标识符进行描述。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ef7004fd7be5340a7e5a1614e51d3ecdfd6f7ff4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024106"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="35b77-104">macOSKernelExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="35b77-104">macOSKernelExtension resource type</span></span>

<span data-ttu-id="35b77-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35b77-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35b77-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35b77-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35b77-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35b77-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35b77-108">表示特定的 macOS 内核扩展。</span><span class="sxs-lookup"><span data-stu-id="35b77-108">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="35b77-109">MacOS 内核扩展可以通过其团队标识符加上其捆绑包标识符进行描述。</span><span class="sxs-lookup"><span data-stu-id="35b77-109">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="35b77-110">属性</span><span class="sxs-lookup"><span data-stu-id="35b77-110">Properties</span></span>
|<span data-ttu-id="35b77-111">属性</span><span class="sxs-lookup"><span data-stu-id="35b77-111">Property</span></span>|<span data-ttu-id="35b77-112">类型</span><span class="sxs-lookup"><span data-stu-id="35b77-112">Type</span></span>|<span data-ttu-id="35b77-113">说明</span><span class="sxs-lookup"><span data-stu-id="35b77-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35b77-114">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="35b77-114">teamIdentifier</span></span>|<span data-ttu-id="35b77-115">String</span><span class="sxs-lookup"><span data-stu-id="35b77-115">String</span></span>|<span data-ttu-id="35b77-116">用于对内核扩展进行签名的团队标识符。</span><span class="sxs-lookup"><span data-stu-id="35b77-116">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="35b77-117">bundleId</span><span class="sxs-lookup"><span data-stu-id="35b77-117">bundleId</span></span>|<span data-ttu-id="35b77-118">String</span><span class="sxs-lookup"><span data-stu-id="35b77-118">String</span></span>|<span data-ttu-id="35b77-119">内核扩展的捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="35b77-119">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35b77-120">关系</span><span class="sxs-lookup"><span data-stu-id="35b77-120">Relationships</span></span>
<span data-ttu-id="35b77-121">无</span><span class="sxs-lookup"><span data-stu-id="35b77-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35b77-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35b77-122">JSON Representation</span></span>
<span data-ttu-id="35b77-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35b77-123">Here is a JSON representation of the resource.</span></span>
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






