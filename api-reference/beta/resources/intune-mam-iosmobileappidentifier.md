---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: tfitzmac
ms.openlocfilehash: e68bfcca4b0873013c0c9e0fd0295483257ae52c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354171"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="acc0d-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="acc0d-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="acc0d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="acc0d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acc0d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="acc0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acc0d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="acc0d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acc0d-107">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="acc0d-107">The identifier for an iOS app.</span></span>

<span data-ttu-id="acc0d-108">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="acc0d-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="acc0d-109">属性</span><span class="sxs-lookup"><span data-stu-id="acc0d-109">Properties</span></span>
|<span data-ttu-id="acc0d-110">属性</span><span class="sxs-lookup"><span data-stu-id="acc0d-110">Property</span></span>|<span data-ttu-id="acc0d-111">类型</span><span class="sxs-lookup"><span data-stu-id="acc0d-111">Type</span></span>|<span data-ttu-id="acc0d-112">说明</span><span class="sxs-lookup"><span data-stu-id="acc0d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acc0d-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="acc0d-113">bundleId</span></span>|<span data-ttu-id="acc0d-114">String</span><span class="sxs-lookup"><span data-stu-id="acc0d-114">String</span></span>|<span data-ttu-id="acc0d-115">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="acc0d-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="acc0d-116">关系</span><span class="sxs-lookup"><span data-stu-id="acc0d-116">Relationships</span></span>
<span data-ttu-id="acc0d-117">无</span><span class="sxs-lookup"><span data-stu-id="acc0d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="acc0d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="acc0d-118">JSON Representation</span></span>
<span data-ttu-id="acc0d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acc0d-119">Here is a JSON representation of the resource.</span></span>
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





