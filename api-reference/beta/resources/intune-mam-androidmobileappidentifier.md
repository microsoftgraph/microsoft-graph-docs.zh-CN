---
title: androidMobileAppIdentifier 资源类型
description: Android 应用的标识符。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 59c947192cf00e1f6852c51513692123595c975b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837588"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="91fb2-103">androidMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="91fb2-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="91fb2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="91fb2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91fb2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="91fb2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91fb2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="91fb2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91fb2-107">Android 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="91fb2-107">The identifier for an Android app.</span></span>

<span data-ttu-id="91fb2-108">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="91fb2-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91fb2-109">属性</span><span class="sxs-lookup"><span data-stu-id="91fb2-109">Properties</span></span>
|<span data-ttu-id="91fb2-110">属性</span><span class="sxs-lookup"><span data-stu-id="91fb2-110">Property</span></span>|<span data-ttu-id="91fb2-111">类型</span><span class="sxs-lookup"><span data-stu-id="91fb2-111">Type</span></span>|<span data-ttu-id="91fb2-112">说明</span><span class="sxs-lookup"><span data-stu-id="91fb2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91fb2-113">packageId</span><span class="sxs-lookup"><span data-stu-id="91fb2-113">packageId</span></span>|<span data-ttu-id="91fb2-114">String</span><span class="sxs-lookup"><span data-stu-id="91fb2-114">String</span></span>|<span data-ttu-id="91fb2-115">应用的标识符，如 Play 商店中指定。</span><span class="sxs-lookup"><span data-stu-id="91fb2-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91fb2-116">关系</span><span class="sxs-lookup"><span data-stu-id="91fb2-116">Relationships</span></span>
<span data-ttu-id="91fb2-117">无</span><span class="sxs-lookup"><span data-stu-id="91fb2-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91fb2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91fb2-118">JSON Representation</span></span>
<span data-ttu-id="91fb2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91fb2-119">Here is a JSON representation of the resource.</span></span>
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





