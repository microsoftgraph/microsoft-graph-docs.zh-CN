---
title: edgeHomeButtonOpensCustomURL 资源类型
description: 显示 "主页" 按钮;单击 "主页" 按钮, 将加载特定的 URL。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88310056a70231c0f536420b87fbecff05b73b42
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001451"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="8e12e-103">edgeHomeButtonOpensCustomURL 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e12e-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="8e12e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8e12e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e12e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e12e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e12e-106">显示 "主页" 按钮;单击 "主页" 按钮, 将加载特定的 URL。</span><span class="sxs-lookup"><span data-stu-id="8e12e-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="8e12e-107">继承自[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e12e-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8e12e-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e12e-108">Properties</span></span>
|<span data-ttu-id="8e12e-109">属性</span><span class="sxs-lookup"><span data-stu-id="8e12e-109">Property</span></span>|<span data-ttu-id="8e12e-110">类型</span><span class="sxs-lookup"><span data-stu-id="8e12e-110">Type</span></span>|<span data-ttu-id="8e12e-111">说明</span><span class="sxs-lookup"><span data-stu-id="8e12e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e12e-112">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="8e12e-112">homeButtonCustomURL</span></span>|<span data-ttu-id="8e12e-113">String</span><span class="sxs-lookup"><span data-stu-id="8e12e-113">String</span></span>|<span data-ttu-id="8e12e-114">要加载的特定 URL。</span><span class="sxs-lookup"><span data-stu-id="8e12e-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e12e-115">关系</span><span class="sxs-lookup"><span data-stu-id="8e12e-115">Relationships</span></span>
<span data-ttu-id="8e12e-116">无</span><span class="sxs-lookup"><span data-stu-id="8e12e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e12e-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e12e-117">JSON Representation</span></span>
<span data-ttu-id="8e12e-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e12e-118">Here is a JSON representation of the resource.</span></span>
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





