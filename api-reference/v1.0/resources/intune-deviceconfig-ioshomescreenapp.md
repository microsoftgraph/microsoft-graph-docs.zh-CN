---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: tfitzmac
ms.openlocfilehash: 68fe4e7b5a226422cc0aaf980ac7fb0421a9bfc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350370"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="d96a0-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="d96a0-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="d96a0-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d96a0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d96a0-105">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="d96a0-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="d96a0-106">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d96a0-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d96a0-107">属性</span><span class="sxs-lookup"><span data-stu-id="d96a0-107">Properties</span></span>
|<span data-ttu-id="d96a0-108">属性</span><span class="sxs-lookup"><span data-stu-id="d96a0-108">Property</span></span>|<span data-ttu-id="d96a0-109">类型</span><span class="sxs-lookup"><span data-stu-id="d96a0-109">Type</span></span>|<span data-ttu-id="d96a0-110">说明</span><span class="sxs-lookup"><span data-stu-id="d96a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d96a0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d96a0-111">displayName</span></span>|<span data-ttu-id="d96a0-112">String</span><span class="sxs-lookup"><span data-stu-id="d96a0-112">String</span></span>|<span data-ttu-id="d96a0-113">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="d96a0-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="d96a0-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="d96a0-114">bundleID</span></span>|<span data-ttu-id="d96a0-115">String</span><span class="sxs-lookup"><span data-stu-id="d96a0-115">String</span></span>|<span data-ttu-id="d96a0-116">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="d96a0-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="d96a0-117">关系</span><span class="sxs-lookup"><span data-stu-id="d96a0-117">Relationships</span></span>
<span data-ttu-id="d96a0-118">无</span><span class="sxs-lookup"><span data-stu-id="d96a0-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d96a0-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d96a0-119">JSON Representation</span></span>
<span data-ttu-id="d96a0-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d96a0-120">Here is a JSON representation of the resource.</span></span>
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



