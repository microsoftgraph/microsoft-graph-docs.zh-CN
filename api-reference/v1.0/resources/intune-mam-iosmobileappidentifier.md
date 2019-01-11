---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5dd2ee1531c2bfe2399949d2e08a209826079cb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875836"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="1a56c-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a56c-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="1a56c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1a56c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a56c-105">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="1a56c-105">The identifier for an iOS app.</span></span>

<span data-ttu-id="1a56c-106">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="1a56c-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a56c-107">属性</span><span class="sxs-lookup"><span data-stu-id="1a56c-107">Properties</span></span>
|<span data-ttu-id="1a56c-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a56c-108">Property</span></span>|<span data-ttu-id="1a56c-109">类型</span><span class="sxs-lookup"><span data-stu-id="1a56c-109">Type</span></span>|<span data-ttu-id="1a56c-110">说明</span><span class="sxs-lookup"><span data-stu-id="1a56c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a56c-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="1a56c-111">bundleId</span></span>|<span data-ttu-id="1a56c-112">String</span><span class="sxs-lookup"><span data-stu-id="1a56c-112">String</span></span>|<span data-ttu-id="1a56c-113">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="1a56c-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a56c-114">关系</span><span class="sxs-lookup"><span data-stu-id="1a56c-114">Relationships</span></span>
<span data-ttu-id="1a56c-115">无</span><span class="sxs-lookup"><span data-stu-id="1a56c-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1a56c-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a56c-116">JSON Representation</span></span>
<span data-ttu-id="1a56c-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a56c-117">Here is a JSON representation of the resource.</span></span>
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



