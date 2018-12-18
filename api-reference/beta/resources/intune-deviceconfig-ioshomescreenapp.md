---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: tfitzmac
ms.openlocfilehash: 63bcfe53cc2d3ee60b5f784e99798f1f97e883af
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334963"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="94edf-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="94edf-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="94edf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="94edf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94edf-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="94edf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94edf-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="94edf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94edf-107">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="94edf-107">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="94edf-108">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="94edf-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="94edf-109">属性</span><span class="sxs-lookup"><span data-stu-id="94edf-109">Properties</span></span>
|<span data-ttu-id="94edf-110">属性</span><span class="sxs-lookup"><span data-stu-id="94edf-110">Property</span></span>|<span data-ttu-id="94edf-111">类型</span><span class="sxs-lookup"><span data-stu-id="94edf-111">Type</span></span>|<span data-ttu-id="94edf-112">说明</span><span class="sxs-lookup"><span data-stu-id="94edf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94edf-113">displayName</span><span class="sxs-lookup"><span data-stu-id="94edf-113">displayName</span></span>|<span data-ttu-id="94edf-114">String</span><span class="sxs-lookup"><span data-stu-id="94edf-114">String</span></span>|<span data-ttu-id="94edf-115">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="94edf-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="94edf-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="94edf-116">bundleID</span></span>|<span data-ttu-id="94edf-117">String</span><span class="sxs-lookup"><span data-stu-id="94edf-117">String</span></span>|<span data-ttu-id="94edf-118">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="94edf-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="94edf-119">关系</span><span class="sxs-lookup"><span data-stu-id="94edf-119">Relationships</span></span>
<span data-ttu-id="94edf-120">无</span><span class="sxs-lookup"><span data-stu-id="94edf-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="94edf-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94edf-121">JSON Representation</span></span>
<span data-ttu-id="94edf-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94edf-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```





