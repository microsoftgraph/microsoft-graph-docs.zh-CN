---
title: androidMobileAppIdentifier 资源类型
description: Android 应用的标识符。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9cc203cc9268849e8b7b46d994c166378252df59
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871741"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="fcebe-103">androidMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="fcebe-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="fcebe-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fcebe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcebe-105">Android 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="fcebe-105">The identifier for an Android app.</span></span>

<span data-ttu-id="fcebe-106">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="fcebe-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fcebe-107">属性</span><span class="sxs-lookup"><span data-stu-id="fcebe-107">Properties</span></span>
|<span data-ttu-id="fcebe-108">属性</span><span class="sxs-lookup"><span data-stu-id="fcebe-108">Property</span></span>|<span data-ttu-id="fcebe-109">类型</span><span class="sxs-lookup"><span data-stu-id="fcebe-109">Type</span></span>|<span data-ttu-id="fcebe-110">说明</span><span class="sxs-lookup"><span data-stu-id="fcebe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcebe-111">packageId</span><span class="sxs-lookup"><span data-stu-id="fcebe-111">packageId</span></span>|<span data-ttu-id="fcebe-112">String</span><span class="sxs-lookup"><span data-stu-id="fcebe-112">String</span></span>|<span data-ttu-id="fcebe-113">应用的标识符，如 Play 商店中指定。</span><span class="sxs-lookup"><span data-stu-id="fcebe-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcebe-114">关系</span><span class="sxs-lookup"><span data-stu-id="fcebe-114">Relationships</span></span>
<span data-ttu-id="fcebe-115">无</span><span class="sxs-lookup"><span data-stu-id="fcebe-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fcebe-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcebe-116">JSON Representation</span></span>
<span data-ttu-id="fcebe-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcebe-117">Here is a JSON representation of the resource.</span></span>
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



