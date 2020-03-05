---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00644356df293ff2171d51bd60c7c5f84748d753
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527969"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="34be7-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="34be7-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="34be7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="34be7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34be7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34be7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34be7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34be7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34be7-107">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="34be7-107">The identifier for an iOS app.</span></span>


<span data-ttu-id="34be7-108">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="34be7-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34be7-109">属性</span><span class="sxs-lookup"><span data-stu-id="34be7-109">Properties</span></span>
|<span data-ttu-id="34be7-110">属性</span><span class="sxs-lookup"><span data-stu-id="34be7-110">Property</span></span>|<span data-ttu-id="34be7-111">类型</span><span class="sxs-lookup"><span data-stu-id="34be7-111">Type</span></span>|<span data-ttu-id="34be7-112">说明</span><span class="sxs-lookup"><span data-stu-id="34be7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34be7-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="34be7-113">bundleId</span></span>|<span data-ttu-id="34be7-114">String</span><span class="sxs-lookup"><span data-stu-id="34be7-114">String</span></span>|<span data-ttu-id="34be7-115">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="34be7-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34be7-116">关系</span><span class="sxs-lookup"><span data-stu-id="34be7-116">Relationships</span></span>
<span data-ttu-id="34be7-117">无</span><span class="sxs-lookup"><span data-stu-id="34be7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34be7-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34be7-118">JSON Representation</span></span>
<span data-ttu-id="34be7-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34be7-119">Here is a JSON representation of the resource.</span></span>
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



