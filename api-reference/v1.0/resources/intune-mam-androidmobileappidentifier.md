---
title: androidMobileAppIdentifier 资源类型
description: Android 应用的标识符。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa3a0f90626ea01290ccd1d0eee3873374efb546
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551846"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="504b1-103">androidMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="504b1-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="504b1-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="504b1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="504b1-105">Android 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="504b1-105">The identifier for an Android app.</span></span>


<span data-ttu-id="504b1-106">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="504b1-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="504b1-107">属性</span><span class="sxs-lookup"><span data-stu-id="504b1-107">Properties</span></span>
|<span data-ttu-id="504b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="504b1-108">Property</span></span>|<span data-ttu-id="504b1-109">类型</span><span class="sxs-lookup"><span data-stu-id="504b1-109">Type</span></span>|<span data-ttu-id="504b1-110">说明</span><span class="sxs-lookup"><span data-stu-id="504b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="504b1-111">packageId</span><span class="sxs-lookup"><span data-stu-id="504b1-111">packageId</span></span>|<span data-ttu-id="504b1-112">String</span><span class="sxs-lookup"><span data-stu-id="504b1-112">String</span></span>|<span data-ttu-id="504b1-113">应用的标识符，如 Play 商店中指定。</span><span class="sxs-lookup"><span data-stu-id="504b1-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="504b1-114">关系</span><span class="sxs-lookup"><span data-stu-id="504b1-114">Relationships</span></span>
<span data-ttu-id="504b1-115">无</span><span class="sxs-lookup"><span data-stu-id="504b1-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="504b1-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="504b1-116">JSON Representation</span></span>
<span data-ttu-id="504b1-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="504b1-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```



