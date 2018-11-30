---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
ms.openlocfilehash: ff749f7166da2d20bfd632e0c595b33f7b1e9fad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010376"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="a1bda-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1bda-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="a1bda-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a1bda-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1bda-105">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="a1bda-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="a1bda-106">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a1bda-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a1bda-107">属性</span><span class="sxs-lookup"><span data-stu-id="a1bda-107">Properties</span></span>
|<span data-ttu-id="a1bda-108">属性</span><span class="sxs-lookup"><span data-stu-id="a1bda-108">Property</span></span>|<span data-ttu-id="a1bda-109">类型</span><span class="sxs-lookup"><span data-stu-id="a1bda-109">Type</span></span>|<span data-ttu-id="a1bda-110">说明</span><span class="sxs-lookup"><span data-stu-id="a1bda-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1bda-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a1bda-111">displayName</span></span>|<span data-ttu-id="a1bda-112">String</span><span class="sxs-lookup"><span data-stu-id="a1bda-112">String</span></span>|<span data-ttu-id="a1bda-113">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="a1bda-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="a1bda-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="a1bda-114">bundleID</span></span>|<span data-ttu-id="a1bda-115">String</span><span class="sxs-lookup"><span data-stu-id="a1bda-115">String</span></span>|<span data-ttu-id="a1bda-116">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="a1bda-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1bda-117">关系</span><span class="sxs-lookup"><span data-stu-id="a1bda-117">Relationships</span></span>
<span data-ttu-id="a1bda-118">无</span><span class="sxs-lookup"><span data-stu-id="a1bda-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a1bda-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1bda-119">JSON Representation</span></span>
<span data-ttu-id="a1bda-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1bda-120">Here is a JSON representation of the resource.</span></span>
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



