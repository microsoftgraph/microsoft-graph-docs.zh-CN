---
title: edgeHomeButtonOpensCustomURL 资源类型
description: 显示 "主页" 按钮;单击 "主页" 按钮，将加载特定的 URL。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60184022f219eba09f205121721b48fd6675d8c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530063"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="1feb8-103">edgeHomeButtonOpensCustomURL 资源类型</span><span class="sxs-lookup"><span data-stu-id="1feb8-103">edgeHomeButtonOpensCustomURL resource type</span></span>

<span data-ttu-id="1feb8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1feb8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1feb8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1feb8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1feb8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1feb8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1feb8-107">显示 "主页" 按钮;单击 "主页" 按钮，将加载特定的 URL。</span><span class="sxs-lookup"><span data-stu-id="1feb8-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="1feb8-108">继承自[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1feb8-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1feb8-109">属性</span><span class="sxs-lookup"><span data-stu-id="1feb8-109">Properties</span></span>
|<span data-ttu-id="1feb8-110">属性</span><span class="sxs-lookup"><span data-stu-id="1feb8-110">Property</span></span>|<span data-ttu-id="1feb8-111">类型</span><span class="sxs-lookup"><span data-stu-id="1feb8-111">Type</span></span>|<span data-ttu-id="1feb8-112">说明</span><span class="sxs-lookup"><span data-stu-id="1feb8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1feb8-113">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="1feb8-113">homeButtonCustomURL</span></span>|<span data-ttu-id="1feb8-114">String</span><span class="sxs-lookup"><span data-stu-id="1feb8-114">String</span></span>|<span data-ttu-id="1feb8-115">要加载的特定 URL。</span><span class="sxs-lookup"><span data-stu-id="1feb8-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1feb8-116">关系</span><span class="sxs-lookup"><span data-stu-id="1feb8-116">Relationships</span></span>
<span data-ttu-id="1feb8-117">无</span><span class="sxs-lookup"><span data-stu-id="1feb8-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1feb8-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1feb8-118">JSON Representation</span></span>
<span data-ttu-id="1feb8-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1feb8-119">Here is a JSON representation of the resource.</span></span>
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



