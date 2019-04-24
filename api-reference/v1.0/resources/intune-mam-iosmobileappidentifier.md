---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb0eaade90c88cc553072f30dd36c42db4f44513
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465417"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="09151-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="09151-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="09151-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09151-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09151-105">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="09151-105">The identifier for an iOS app.</span></span>


<span data-ttu-id="09151-106">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="09151-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09151-107">属性</span><span class="sxs-lookup"><span data-stu-id="09151-107">Properties</span></span>
|<span data-ttu-id="09151-108">属性</span><span class="sxs-lookup"><span data-stu-id="09151-108">Property</span></span>|<span data-ttu-id="09151-109">类型</span><span class="sxs-lookup"><span data-stu-id="09151-109">Type</span></span>|<span data-ttu-id="09151-110">说明</span><span class="sxs-lookup"><span data-stu-id="09151-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09151-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="09151-111">bundleId</span></span>|<span data-ttu-id="09151-112">String</span><span class="sxs-lookup"><span data-stu-id="09151-112">String</span></span>|<span data-ttu-id="09151-113">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="09151-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09151-114">关系</span><span class="sxs-lookup"><span data-stu-id="09151-114">Relationships</span></span>
<span data-ttu-id="09151-115">无</span><span class="sxs-lookup"><span data-stu-id="09151-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09151-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09151-116">JSON Representation</span></span>
<span data-ttu-id="09151-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09151-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```



