---
title: androidMobileAppIdentifier 资源类型
description: Android 应用的标识符。
author: tfitzmac
ms.openlocfilehash: fa55d84c3f676d23caeba1e5fda33166b60aaada
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350825"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="7b73b-103">androidMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b73b-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="7b73b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7b73b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b73b-105">Android 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="7b73b-105">The identifier for an Android app.</span></span>

<span data-ttu-id="7b73b-106">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="7b73b-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7b73b-107">属性</span><span class="sxs-lookup"><span data-stu-id="7b73b-107">Properties</span></span>
|<span data-ttu-id="7b73b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7b73b-108">Property</span></span>|<span data-ttu-id="7b73b-109">类型</span><span class="sxs-lookup"><span data-stu-id="7b73b-109">Type</span></span>|<span data-ttu-id="7b73b-110">说明</span><span class="sxs-lookup"><span data-stu-id="7b73b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b73b-111">packageId</span><span class="sxs-lookup"><span data-stu-id="7b73b-111">packageId</span></span>|<span data-ttu-id="7b73b-112">String</span><span class="sxs-lookup"><span data-stu-id="7b73b-112">String</span></span>|<span data-ttu-id="7b73b-113">应用的标识符，如 Play 商店中指定。</span><span class="sxs-lookup"><span data-stu-id="7b73b-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b73b-114">关系</span><span class="sxs-lookup"><span data-stu-id="7b73b-114">Relationships</span></span>
<span data-ttu-id="7b73b-115">无</span><span class="sxs-lookup"><span data-stu-id="7b73b-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7b73b-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b73b-116">JSON Representation</span></span>
<span data-ttu-id="7b73b-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b73b-117">Here is a JSON representation of the resource.</span></span>
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



