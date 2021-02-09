---
title: macAppIdentifier 资源类型
description: Mac 应用的标识符。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4ee44dc2fe288d7a1605660ef95dc7d88f600fb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160521"
---
# <a name="macappidentifier-resource-type"></a><span data-ttu-id="4e13d-103">macAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e13d-103">macAppIdentifier resource type</span></span>

<span data-ttu-id="4e13d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e13d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e13d-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e13d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e13d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e13d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e13d-107">Mac 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="4e13d-107">The identifier for a Mac app.</span></span>


<span data-ttu-id="4e13d-108">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="4e13d-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e13d-109">属性</span><span class="sxs-lookup"><span data-stu-id="4e13d-109">Properties</span></span>
|<span data-ttu-id="4e13d-110">属性</span><span class="sxs-lookup"><span data-stu-id="4e13d-110">Property</span></span>|<span data-ttu-id="4e13d-111">类型</span><span class="sxs-lookup"><span data-stu-id="4e13d-111">Type</span></span>|<span data-ttu-id="4e13d-112">说明</span><span class="sxs-lookup"><span data-stu-id="4e13d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e13d-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="4e13d-113">bundleId</span></span>|<span data-ttu-id="4e13d-114">String</span><span class="sxs-lookup"><span data-stu-id="4e13d-114">String</span></span>|<span data-ttu-id="4e13d-115">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="4e13d-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e13d-116">关系</span><span class="sxs-lookup"><span data-stu-id="4e13d-116">Relationships</span></span>
<span data-ttu-id="4e13d-117">无</span><span class="sxs-lookup"><span data-stu-id="4e13d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e13d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e13d-118">JSON Representation</span></span>
<span data-ttu-id="4e13d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e13d-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macAppIdentifier",
  "bundleId": "String"
}
```




