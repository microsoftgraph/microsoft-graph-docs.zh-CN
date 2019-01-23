---
title: edgeHomeButtonOpensCustomURL 资源类型
description: 显示主页按钮。单击主页按钮加载特定的 URL。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 06f73375772f53b546e7e9b758a7513366949326
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431405"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="63855-103">edgeHomeButtonOpensCustomURL 资源类型</span><span class="sxs-lookup"><span data-stu-id="63855-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="63855-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="63855-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63855-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="63855-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63855-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63855-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63855-107">显示主页按钮。单击主页按钮加载特定的 URL。</span><span class="sxs-lookup"><span data-stu-id="63855-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="63855-108">继承自[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63855-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="63855-109">属性</span><span class="sxs-lookup"><span data-stu-id="63855-109">Properties</span></span>
|<span data-ttu-id="63855-110">属性</span><span class="sxs-lookup"><span data-stu-id="63855-110">Property</span></span>|<span data-ttu-id="63855-111">类型</span><span class="sxs-lookup"><span data-stu-id="63855-111">Type</span></span>|<span data-ttu-id="63855-112">说明</span><span class="sxs-lookup"><span data-stu-id="63855-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63855-113">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="63855-113">homeButtonCustomURL</span></span>|<span data-ttu-id="63855-114">String</span><span class="sxs-lookup"><span data-stu-id="63855-114">String</span></span>|<span data-ttu-id="63855-115">要加载的特定 URL。</span><span class="sxs-lookup"><span data-stu-id="63855-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63855-116">关系</span><span class="sxs-lookup"><span data-stu-id="63855-116">Relationships</span></span>
<span data-ttu-id="63855-117">无</span><span class="sxs-lookup"><span data-stu-id="63855-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63855-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63855-118">JSON Representation</span></span>
<span data-ttu-id="63855-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63855-119">Here is a JSON representation of the resource.</span></span>
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




