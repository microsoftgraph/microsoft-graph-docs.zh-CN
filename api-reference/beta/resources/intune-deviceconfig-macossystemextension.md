---
title: macOSSystemExtension 资源类型
description: 表示特定的 macOS 系统扩展。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f72b2856d95205e17c8bfdf45974676ea9644fa6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064134"
---
# <a name="macossystemextension-resource-type"></a><span data-ttu-id="bac26-103">macOSSystemExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="bac26-103">macOSSystemExtension resource type</span></span>

<span data-ttu-id="bac26-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bac26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bac26-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bac26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bac26-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bac26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bac26-107">表示特定的 macOS 系统扩展。</span><span class="sxs-lookup"><span data-stu-id="bac26-107">Represents a specific macOS system extension.</span></span>

## <a name="properties"></a><span data-ttu-id="bac26-108">属性</span><span class="sxs-lookup"><span data-stu-id="bac26-108">Properties</span></span>
|<span data-ttu-id="bac26-109">属性</span><span class="sxs-lookup"><span data-stu-id="bac26-109">Property</span></span>|<span data-ttu-id="bac26-110">类型</span><span class="sxs-lookup"><span data-stu-id="bac26-110">Type</span></span>|<span data-ttu-id="bac26-111">说明</span><span class="sxs-lookup"><span data-stu-id="bac26-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bac26-112">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="bac26-112">teamIdentifier</span></span>|<span data-ttu-id="bac26-113">String</span><span class="sxs-lookup"><span data-stu-id="bac26-113">String</span></span>|<span data-ttu-id="bac26-114">获取或设置用于对系统扩展进行签名的团队标识符。</span><span class="sxs-lookup"><span data-stu-id="bac26-114">Gets or sets the team identifier that was used to sign the system extension.</span></span>|
|<span data-ttu-id="bac26-115">bundleId</span><span class="sxs-lookup"><span data-stu-id="bac26-115">bundleId</span></span>|<span data-ttu-id="bac26-116">String</span><span class="sxs-lookup"><span data-stu-id="bac26-116">String</span></span>|<span data-ttu-id="bac26-117">获取或设置系统扩展的捆绑包标识符。</span><span class="sxs-lookup"><span data-stu-id="bac26-117">Gets or sets the bundle identifier of the system extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bac26-118">关系</span><span class="sxs-lookup"><span data-stu-id="bac26-118">Relationships</span></span>
<span data-ttu-id="bac26-119">无</span><span class="sxs-lookup"><span data-stu-id="bac26-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bac26-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bac26-120">JSON Representation</span></span>
<span data-ttu-id="bac26-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bac26-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```






