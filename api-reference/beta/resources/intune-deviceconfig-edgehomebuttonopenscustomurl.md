---
title: edgeHomeButtonOpensCustomURL 资源类型
description: 显示 "主页" 按钮;单击 "主页" 按钮, 将加载特定的 URL。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e83fd3dbb0961011584ef9d65e01c361ccf6a228
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143237"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="252cc-103">edgeHomeButtonOpensCustomURL 资源类型</span><span class="sxs-lookup"><span data-stu-id="252cc-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="252cc-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="252cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="252cc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="252cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="252cc-106">显示 "主页" 按钮;单击 "主页" 按钮, 将加载特定的 URL。</span><span class="sxs-lookup"><span data-stu-id="252cc-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="252cc-107">继承自[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="252cc-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="252cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="252cc-108">Properties</span></span>
|<span data-ttu-id="252cc-109">属性</span><span class="sxs-lookup"><span data-stu-id="252cc-109">Property</span></span>|<span data-ttu-id="252cc-110">类型</span><span class="sxs-lookup"><span data-stu-id="252cc-110">Type</span></span>|<span data-ttu-id="252cc-111">说明</span><span class="sxs-lookup"><span data-stu-id="252cc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="252cc-112">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="252cc-112">homeButtonCustomURL</span></span>|<span data-ttu-id="252cc-113">字符串</span><span class="sxs-lookup"><span data-stu-id="252cc-113">String</span></span>|<span data-ttu-id="252cc-114">要加载的特定 URL。</span><span class="sxs-lookup"><span data-stu-id="252cc-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="252cc-115">关系</span><span class="sxs-lookup"><span data-stu-id="252cc-115">Relationships</span></span>
<span data-ttu-id="252cc-116">无</span><span class="sxs-lookup"><span data-stu-id="252cc-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="252cc-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="252cc-117">JSON Representation</span></span>
<span data-ttu-id="252cc-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="252cc-118">Here is a JSON representation of the resource.</span></span>
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




