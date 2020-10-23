---
title: edgeHomeButtonOpensCustomURL 资源类型
description: 显示 "主页" 按钮;单击 "主页" 按钮，将加载特定的 URL。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f6bd4db13fad2863ffa6661fb9273085f70b7c0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732584"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="00066-103">edgeHomeButtonOpensCustomURL 资源类型</span><span class="sxs-lookup"><span data-stu-id="00066-103">edgeHomeButtonOpensCustomURL resource type</span></span>

<span data-ttu-id="00066-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00066-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00066-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="00066-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00066-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="00066-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00066-107">显示 "主页" 按钮;单击 "主页" 按钮，将加载特定的 URL。</span><span class="sxs-lookup"><span data-stu-id="00066-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="00066-108">继承自 [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00066-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="00066-109">属性</span><span class="sxs-lookup"><span data-stu-id="00066-109">Properties</span></span>
|<span data-ttu-id="00066-110">属性</span><span class="sxs-lookup"><span data-stu-id="00066-110">Property</span></span>|<span data-ttu-id="00066-111">类型</span><span class="sxs-lookup"><span data-stu-id="00066-111">Type</span></span>|<span data-ttu-id="00066-112">说明</span><span class="sxs-lookup"><span data-stu-id="00066-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00066-113">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="00066-113">homeButtonCustomURL</span></span>|<span data-ttu-id="00066-114">String</span><span class="sxs-lookup"><span data-stu-id="00066-114">String</span></span>|<span data-ttu-id="00066-115">要加载的特定 URL。</span><span class="sxs-lookup"><span data-stu-id="00066-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00066-116">关系</span><span class="sxs-lookup"><span data-stu-id="00066-116">Relationships</span></span>
<span data-ttu-id="00066-117">无</span><span class="sxs-lookup"><span data-stu-id="00066-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00066-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00066-118">JSON Representation</span></span>
<span data-ttu-id="00066-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00066-119">Here is a JSON representation of the resource.</span></span>
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





