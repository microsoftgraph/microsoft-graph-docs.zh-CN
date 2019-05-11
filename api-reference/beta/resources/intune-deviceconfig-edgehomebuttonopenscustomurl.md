---
title: edgeHomeButtonOpensCustomURL 资源类型
description: 显示 "主页" 按钮;单击 "主页" 按钮, 将加载特定的 URL。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3b82acaf8ef5f6e008d759f257c7382ff64492b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946817"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="71f55-103">edgeHomeButtonOpensCustomURL 资源类型</span><span class="sxs-lookup"><span data-stu-id="71f55-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="71f55-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="71f55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71f55-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71f55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71f55-106">显示 "主页" 按钮;单击 "主页" 按钮, 将加载特定的 URL。</span><span class="sxs-lookup"><span data-stu-id="71f55-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="71f55-107">继承自[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71f55-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="71f55-108">属性</span><span class="sxs-lookup"><span data-stu-id="71f55-108">Properties</span></span>
|<span data-ttu-id="71f55-109">属性</span><span class="sxs-lookup"><span data-stu-id="71f55-109">Property</span></span>|<span data-ttu-id="71f55-110">类型</span><span class="sxs-lookup"><span data-stu-id="71f55-110">Type</span></span>|<span data-ttu-id="71f55-111">说明</span><span class="sxs-lookup"><span data-stu-id="71f55-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71f55-112">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="71f55-112">homeButtonCustomURL</span></span>|<span data-ttu-id="71f55-113">String</span><span class="sxs-lookup"><span data-stu-id="71f55-113">String</span></span>|<span data-ttu-id="71f55-114">要加载的特定 URL。</span><span class="sxs-lookup"><span data-stu-id="71f55-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71f55-115">关系</span><span class="sxs-lookup"><span data-stu-id="71f55-115">Relationships</span></span>
<span data-ttu-id="71f55-116">无</span><span class="sxs-lookup"><span data-stu-id="71f55-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71f55-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71f55-117">JSON Representation</span></span>
<span data-ttu-id="71f55-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71f55-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```




