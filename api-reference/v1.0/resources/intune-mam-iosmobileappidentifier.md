---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0ab8119fec6998e9aaa06d2de0cf10b991a5b139
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984409"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="0fe9c-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fe9c-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="0fe9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fe9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fe9c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0fe9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fe9c-106">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="0fe9c-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="0fe9c-107">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="0fe9c-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0fe9c-108">属性</span><span class="sxs-lookup"><span data-stu-id="0fe9c-108">Properties</span></span>
|<span data-ttu-id="0fe9c-109">属性</span><span class="sxs-lookup"><span data-stu-id="0fe9c-109">Property</span></span>|<span data-ttu-id="0fe9c-110">类型</span><span class="sxs-lookup"><span data-stu-id="0fe9c-110">Type</span></span>|<span data-ttu-id="0fe9c-111">说明</span><span class="sxs-lookup"><span data-stu-id="0fe9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fe9c-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="0fe9c-112">bundleId</span></span>|<span data-ttu-id="0fe9c-113">String</span><span class="sxs-lookup"><span data-stu-id="0fe9c-113">String</span></span>|<span data-ttu-id="0fe9c-114">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="0fe9c-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fe9c-115">关系</span><span class="sxs-lookup"><span data-stu-id="0fe9c-115">Relationships</span></span>
<span data-ttu-id="0fe9c-116">无</span><span class="sxs-lookup"><span data-stu-id="0fe9c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fe9c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fe9c-117">JSON Representation</span></span>
<span data-ttu-id="0fe9c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fe9c-118">Here is a JSON representation of the resource.</span></span>
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









