---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 190726b8ee7411a5ce53f8e2802ddf38e0e6b9ff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408416"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="9bb3d-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="9bb3d-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="9bb3d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9bb3d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9bb3d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9bb3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9bb3d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9bb3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bb3d-107">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="9bb3d-107">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="9bb3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="9bb3d-108">Properties</span></span>
|<span data-ttu-id="9bb3d-109">属性</span><span class="sxs-lookup"><span data-stu-id="9bb3d-109">Property</span></span>|<span data-ttu-id="9bb3d-110">类型</span><span class="sxs-lookup"><span data-stu-id="9bb3d-110">Type</span></span>|<span data-ttu-id="9bb3d-111">说明</span><span class="sxs-lookup"><span data-stu-id="9bb3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bb3d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9bb3d-112">displayName</span></span>|<span data-ttu-id="9bb3d-113">String</span><span class="sxs-lookup"><span data-stu-id="9bb3d-113">String</span></span>|<span data-ttu-id="9bb3d-114">应用的名称</span><span class="sxs-lookup"><span data-stu-id="9bb3d-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="9bb3d-115">关系</span><span class="sxs-lookup"><span data-stu-id="9bb3d-115">Relationships</span></span>
<span data-ttu-id="9bb3d-116">无</span><span class="sxs-lookup"><span data-stu-id="9bb3d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9bb3d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9bb3d-117">JSON Representation</span></span>
<span data-ttu-id="9bb3d-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9bb3d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```




