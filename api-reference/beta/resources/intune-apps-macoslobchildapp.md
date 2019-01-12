---
title: macOSLobChildApp 资源类型
description: 包含 MacOS LOB 应用程序中绑定包中属性
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43f207bb2cebccdd01c791694674c6fbf96b631f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954230"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="9c59f-103">macOSLobChildApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c59f-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="9c59f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9c59f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c59f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9c59f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c59f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9c59f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c59f-107">包含 MacOS LOB 应用程序中绑定包中属性</span><span class="sxs-lookup"><span data-stu-id="9c59f-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="9c59f-108">属性</span><span class="sxs-lookup"><span data-stu-id="9c59f-108">Properties</span></span>
|<span data-ttu-id="9c59f-109">属性</span><span class="sxs-lookup"><span data-stu-id="9c59f-109">Property</span></span>|<span data-ttu-id="9c59f-110">类型</span><span class="sxs-lookup"><span data-stu-id="9c59f-110">Type</span></span>|<span data-ttu-id="9c59f-111">说明</span><span class="sxs-lookup"><span data-stu-id="9c59f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c59f-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="9c59f-112">bundleId</span></span>|<span data-ttu-id="9c59f-113">String</span><span class="sxs-lookup"><span data-stu-id="9c59f-113">String</span></span>|<span data-ttu-id="9c59f-114">标识名称。</span><span class="sxs-lookup"><span data-stu-id="9c59f-114">The Identity Name.</span></span>|
|<span data-ttu-id="9c59f-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="9c59f-115">buildNumber</span></span>|<span data-ttu-id="9c59f-116">String</span><span class="sxs-lookup"><span data-stu-id="9c59f-116">String</span></span>|<span data-ttu-id="9c59f-117">MacOS 行业务 (LoB) 应用程序的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="9c59f-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9c59f-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="9c59f-118">versionNumber</span></span>|<span data-ttu-id="9c59f-119">String</span><span class="sxs-lookup"><span data-stu-id="9c59f-119">String</span></span>|<span data-ttu-id="9c59f-120">MacOS 线 (LoB) 企业应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="9c59f-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c59f-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="9c59f-121">Relationships</span></span>
<span data-ttu-id="9c59f-122">无</span><span class="sxs-lookup"><span data-stu-id="9c59f-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9c59f-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c59f-123">JSON Representation</span></span>
<span data-ttu-id="9c59f-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c59f-124">Here is a JSON representation of the resource.</span></span>
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





