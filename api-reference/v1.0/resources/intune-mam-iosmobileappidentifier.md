---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b1dbebd30fecd15a916eef554bbdffd27b435f3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754523"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="41f97-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="41f97-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="41f97-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41f97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41f97-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41f97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41f97-106">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="41f97-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="41f97-107">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="41f97-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="41f97-108">属性</span><span class="sxs-lookup"><span data-stu-id="41f97-108">Properties</span></span>
|<span data-ttu-id="41f97-109">属性</span><span class="sxs-lookup"><span data-stu-id="41f97-109">Property</span></span>|<span data-ttu-id="41f97-110">类型</span><span class="sxs-lookup"><span data-stu-id="41f97-110">Type</span></span>|<span data-ttu-id="41f97-111">Description</span><span class="sxs-lookup"><span data-stu-id="41f97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41f97-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="41f97-112">bundleId</span></span>|<span data-ttu-id="41f97-113">String</span><span class="sxs-lookup"><span data-stu-id="41f97-113">String</span></span>|<span data-ttu-id="41f97-114">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="41f97-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41f97-115">关系</span><span class="sxs-lookup"><span data-stu-id="41f97-115">Relationships</span></span>
<span data-ttu-id="41f97-116">无</span><span class="sxs-lookup"><span data-stu-id="41f97-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41f97-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41f97-117">JSON Representation</span></span>
<span data-ttu-id="41f97-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41f97-118">Here is a JSON representation of the resource.</span></span>
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




