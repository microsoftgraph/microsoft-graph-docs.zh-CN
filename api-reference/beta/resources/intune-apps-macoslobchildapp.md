---
title: macOSLobChildApp 资源类型
description: 包含 MacOS LOB 应用程序中绑定包中属性
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a6a8cafc0f9b47f40fe7e922130a41d37a427e5e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403019"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="9f34c-103">macOSLobChildApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f34c-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="9f34c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9f34c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9f34c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9f34c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f34c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f34c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f34c-107">包含 MacOS LOB 应用程序中绑定包中属性</span><span class="sxs-lookup"><span data-stu-id="9f34c-107">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="9f34c-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f34c-108">Properties</span></span>
|<span data-ttu-id="9f34c-109">属性</span><span class="sxs-lookup"><span data-stu-id="9f34c-109">Property</span></span>|<span data-ttu-id="9f34c-110">类型</span><span class="sxs-lookup"><span data-stu-id="9f34c-110">Type</span></span>|<span data-ttu-id="9f34c-111">说明</span><span class="sxs-lookup"><span data-stu-id="9f34c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f34c-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="9f34c-112">bundleId</span></span>|<span data-ttu-id="9f34c-113">String</span><span class="sxs-lookup"><span data-stu-id="9f34c-113">String</span></span>|<span data-ttu-id="9f34c-114">标识名称。</span><span class="sxs-lookup"><span data-stu-id="9f34c-114">The Identity Name.</span></span>|
|<span data-ttu-id="9f34c-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="9f34c-115">buildNumber</span></span>|<span data-ttu-id="9f34c-116">String</span><span class="sxs-lookup"><span data-stu-id="9f34c-116">String</span></span>|<span data-ttu-id="9f34c-117">MacOS 行业务 (LoB) 应用程序的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="9f34c-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9f34c-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="9f34c-118">versionNumber</span></span>|<span data-ttu-id="9f34c-119">String</span><span class="sxs-lookup"><span data-stu-id="9f34c-119">String</span></span>|<span data-ttu-id="9f34c-120">MacOS 线 (LoB) 企业应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="9f34c-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f34c-121">关系</span><span class="sxs-lookup"><span data-stu-id="9f34c-121">Relationships</span></span>
<span data-ttu-id="9f34c-122">无</span><span class="sxs-lookup"><span data-stu-id="9f34c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f34c-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f34c-123">JSON Representation</span></span>
<span data-ttu-id="9f34c-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f34c-124">Here is a JSON representation of the resource.</span></span>
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




