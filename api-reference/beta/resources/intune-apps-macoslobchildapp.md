---
title: macOSLobChildApp 资源类型
description: 包含 MacOS LOB 应用程序中绑定包中属性
author: tfitzmac
ms.openlocfilehash: e62305ea856d42847b49be306d20bde737152163
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309868"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="b5299-103">macOSLobChildApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5299-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="b5299-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b5299-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5299-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b5299-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5299-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b5299-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5299-107">包含 MacOS LOB 应用程序中绑定包中属性</span><span class="sxs-lookup"><span data-stu-id="b5299-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="b5299-108">属性</span><span class="sxs-lookup"><span data-stu-id="b5299-108">Properties</span></span>
|<span data-ttu-id="b5299-109">属性</span><span class="sxs-lookup"><span data-stu-id="b5299-109">Property</span></span>|<span data-ttu-id="b5299-110">类型</span><span class="sxs-lookup"><span data-stu-id="b5299-110">Type</span></span>|<span data-ttu-id="b5299-111">说明</span><span class="sxs-lookup"><span data-stu-id="b5299-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5299-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="b5299-112">bundleId</span></span>|<span data-ttu-id="b5299-113">String</span><span class="sxs-lookup"><span data-stu-id="b5299-113">String</span></span>|<span data-ttu-id="b5299-114">标识名称。</span><span class="sxs-lookup"><span data-stu-id="b5299-114">The Identity Name.</span></span>|
|<span data-ttu-id="b5299-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="b5299-115">buildNumber</span></span>|<span data-ttu-id="b5299-116">String</span><span class="sxs-lookup"><span data-stu-id="b5299-116">String</span></span>|<span data-ttu-id="b5299-117">MacOS 行业务 (LoB) 应用程序的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="b5299-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b5299-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="b5299-118">versionNumber</span></span>|<span data-ttu-id="b5299-119">String</span><span class="sxs-lookup"><span data-stu-id="b5299-119">String</span></span>|<span data-ttu-id="b5299-120">MacOS 线 (LoB) 企业应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="b5299-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5299-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="b5299-121">Relationships</span></span>
<span data-ttu-id="b5299-122">无</span><span class="sxs-lookup"><span data-stu-id="b5299-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5299-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5299-123">JSON Representation</span></span>
<span data-ttu-id="b5299-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5299-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```





