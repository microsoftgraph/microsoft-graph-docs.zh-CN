---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 134f6e27b6fb113516fd119211e245fd77b2ae75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919524"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="ab7df-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab7df-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="ab7df-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ab7df-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab7df-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ab7df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab7df-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ab7df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab7df-107">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="ab7df-107">The identifier for an iOS app.</span></span>

<span data-ttu-id="ab7df-108">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="ab7df-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ab7df-109">属性</span><span class="sxs-lookup"><span data-stu-id="ab7df-109">Properties</span></span>
|<span data-ttu-id="ab7df-110">属性</span><span class="sxs-lookup"><span data-stu-id="ab7df-110">Property</span></span>|<span data-ttu-id="ab7df-111">类型</span><span class="sxs-lookup"><span data-stu-id="ab7df-111">Type</span></span>|<span data-ttu-id="ab7df-112">说明</span><span class="sxs-lookup"><span data-stu-id="ab7df-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab7df-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="ab7df-113">bundleId</span></span>|<span data-ttu-id="ab7df-114">String</span><span class="sxs-lookup"><span data-stu-id="ab7df-114">String</span></span>|<span data-ttu-id="ab7df-115">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="ab7df-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab7df-116">关系</span><span class="sxs-lookup"><span data-stu-id="ab7df-116">Relationships</span></span>
<span data-ttu-id="ab7df-117">无</span><span class="sxs-lookup"><span data-stu-id="ab7df-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ab7df-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab7df-118">JSON Representation</span></span>
<span data-ttu-id="ab7df-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab7df-119">Here is a JSON representation of the resource.</span></span>
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





