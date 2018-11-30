---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
ms.openlocfilehash: dbf37da4f225a42b1686896e3fa1fafa472b4a67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010880"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="1116c-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="1116c-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="1116c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1116c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1116c-105">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="1116c-105">The identifier for an iOS app.</span></span>

<span data-ttu-id="1116c-106">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="1116c-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1116c-107">属性</span><span class="sxs-lookup"><span data-stu-id="1116c-107">Properties</span></span>
|<span data-ttu-id="1116c-108">属性</span><span class="sxs-lookup"><span data-stu-id="1116c-108">Property</span></span>|<span data-ttu-id="1116c-109">类型</span><span class="sxs-lookup"><span data-stu-id="1116c-109">Type</span></span>|<span data-ttu-id="1116c-110">说明</span><span class="sxs-lookup"><span data-stu-id="1116c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1116c-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="1116c-111">bundleId</span></span>|<span data-ttu-id="1116c-112">String</span><span class="sxs-lookup"><span data-stu-id="1116c-112">String</span></span>|<span data-ttu-id="1116c-113">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="1116c-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1116c-114">关系</span><span class="sxs-lookup"><span data-stu-id="1116c-114">Relationships</span></span>
<span data-ttu-id="1116c-115">无</span><span class="sxs-lookup"><span data-stu-id="1116c-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1116c-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1116c-116">JSON Representation</span></span>
<span data-ttu-id="1116c-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1116c-117">Here is a JSON representation of the resource.</span></span>
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



