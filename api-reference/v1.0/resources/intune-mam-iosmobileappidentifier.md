---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5e9305963654356c56bff31f6ffb9f97129f4980
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922786"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="1db6f-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="1db6f-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="1db6f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1db6f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1db6f-105">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="1db6f-105">The identifier for an iOS app.</span></span>

<span data-ttu-id="1db6f-106">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="1db6f-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1db6f-107">属性</span><span class="sxs-lookup"><span data-stu-id="1db6f-107">Properties</span></span>
|<span data-ttu-id="1db6f-108">属性</span><span class="sxs-lookup"><span data-stu-id="1db6f-108">Property</span></span>|<span data-ttu-id="1db6f-109">类型</span><span class="sxs-lookup"><span data-stu-id="1db6f-109">Type</span></span>|<span data-ttu-id="1db6f-110">说明</span><span class="sxs-lookup"><span data-stu-id="1db6f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1db6f-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="1db6f-111">bundleId</span></span>|<span data-ttu-id="1db6f-112">String</span><span class="sxs-lookup"><span data-stu-id="1db6f-112">String</span></span>|<span data-ttu-id="1db6f-113">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="1db6f-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1db6f-114">关系</span><span class="sxs-lookup"><span data-stu-id="1db6f-114">Relationships</span></span>
<span data-ttu-id="1db6f-115">无</span><span class="sxs-lookup"><span data-stu-id="1db6f-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1db6f-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1db6f-116">JSON Representation</span></span>
<span data-ttu-id="1db6f-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1db6f-117">Here is a JSON representation of the resource.</span></span>
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



