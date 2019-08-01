---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7388e6872eb48d3aba188448c263f492d913f79b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038148"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="5670b-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="5670b-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="5670b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5670b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5670b-105">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="5670b-105">The identifier for an iOS app.</span></span>


<span data-ttu-id="5670b-106">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="5670b-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5670b-107">属性</span><span class="sxs-lookup"><span data-stu-id="5670b-107">Properties</span></span>
|<span data-ttu-id="5670b-108">属性</span><span class="sxs-lookup"><span data-stu-id="5670b-108">Property</span></span>|<span data-ttu-id="5670b-109">类型</span><span class="sxs-lookup"><span data-stu-id="5670b-109">Type</span></span>|<span data-ttu-id="5670b-110">说明</span><span class="sxs-lookup"><span data-stu-id="5670b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5670b-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="5670b-111">bundleId</span></span>|<span data-ttu-id="5670b-112">String</span><span class="sxs-lookup"><span data-stu-id="5670b-112">String</span></span>|<span data-ttu-id="5670b-113">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="5670b-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5670b-114">关系</span><span class="sxs-lookup"><span data-stu-id="5670b-114">Relationships</span></span>
<span data-ttu-id="5670b-115">无</span><span class="sxs-lookup"><span data-stu-id="5670b-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5670b-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5670b-116">JSON Representation</span></span>
<span data-ttu-id="5670b-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5670b-117">Here is a JSON representation of the resource.</span></span>
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



