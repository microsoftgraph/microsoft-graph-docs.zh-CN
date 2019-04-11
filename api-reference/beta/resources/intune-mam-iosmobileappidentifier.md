---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 98486915252e56928da2e70f98e14b5bf5275ecc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789358"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="56544-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="56544-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="56544-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56544-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56544-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56544-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56544-106">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="56544-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="56544-107">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="56544-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56544-108">属性</span><span class="sxs-lookup"><span data-stu-id="56544-108">Properties</span></span>
|<span data-ttu-id="56544-109">属性</span><span class="sxs-lookup"><span data-stu-id="56544-109">Property</span></span>|<span data-ttu-id="56544-110">类型</span><span class="sxs-lookup"><span data-stu-id="56544-110">Type</span></span>|<span data-ttu-id="56544-111">说明</span><span class="sxs-lookup"><span data-stu-id="56544-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56544-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="56544-112">bundleId</span></span>|<span data-ttu-id="56544-113">String</span><span class="sxs-lookup"><span data-stu-id="56544-113">String</span></span>|<span data-ttu-id="56544-114">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="56544-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56544-115">关系</span><span class="sxs-lookup"><span data-stu-id="56544-115">Relationships</span></span>
<span data-ttu-id="56544-116">无</span><span class="sxs-lookup"><span data-stu-id="56544-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56544-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56544-117">JSON Representation</span></span>
<span data-ttu-id="56544-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56544-118">Here is a JSON representation of the resource.</span></span>
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





