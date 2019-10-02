---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c85d0f1a2bedffe8525c2012487646c4364ec2ff
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356497"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="cef56-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="cef56-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="cef56-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cef56-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cef56-105">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="cef56-105">The identifier for an iOS app.</span></span>


<span data-ttu-id="cef56-106">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="cef56-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cef56-107">属性</span><span class="sxs-lookup"><span data-stu-id="cef56-107">Properties</span></span>
|<span data-ttu-id="cef56-108">属性</span><span class="sxs-lookup"><span data-stu-id="cef56-108">Property</span></span>|<span data-ttu-id="cef56-109">类型</span><span class="sxs-lookup"><span data-stu-id="cef56-109">Type</span></span>|<span data-ttu-id="cef56-110">说明</span><span class="sxs-lookup"><span data-stu-id="cef56-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cef56-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="cef56-111">bundleId</span></span>|<span data-ttu-id="cef56-112">String</span><span class="sxs-lookup"><span data-stu-id="cef56-112">String</span></span>|<span data-ttu-id="cef56-113">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="cef56-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cef56-114">关系</span><span class="sxs-lookup"><span data-stu-id="cef56-114">Relationships</span></span>
<span data-ttu-id="cef56-115">无</span><span class="sxs-lookup"><span data-stu-id="cef56-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cef56-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cef56-116">JSON Representation</span></span>
<span data-ttu-id="cef56-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cef56-117">Here is a JSON representation of the resource.</span></span>
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




