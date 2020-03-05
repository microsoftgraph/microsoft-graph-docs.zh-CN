---
title: win32LobAppProductCodeDetection 资源类型
description: 包含用于检测 Win32 应用程序的产品代码和版本属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c9cccd7dd1e5963b495503286a8f6985b8e359dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490495"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="551cb-103">win32LobAppProductCodeDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="551cb-103">win32LobAppProductCodeDetection resource type</span></span>

<span data-ttu-id="551cb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="551cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="551cb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="551cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="551cb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="551cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="551cb-107">包含用于检测 Win32 应用程序的产品代码和版本属性</span><span class="sxs-lookup"><span data-stu-id="551cb-107">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="551cb-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="551cb-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="551cb-109">属性</span><span class="sxs-lookup"><span data-stu-id="551cb-109">Properties</span></span>
|<span data-ttu-id="551cb-110">属性</span><span class="sxs-lookup"><span data-stu-id="551cb-110">Property</span></span>|<span data-ttu-id="551cb-111">类型</span><span class="sxs-lookup"><span data-stu-id="551cb-111">Type</span></span>|<span data-ttu-id="551cb-112">说明</span><span class="sxs-lookup"><span data-stu-id="551cb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="551cb-113">productCode</span><span class="sxs-lookup"><span data-stu-id="551cb-113">productCode</span></span>|<span data-ttu-id="551cb-114">String</span><span class="sxs-lookup"><span data-stu-id="551cb-114">String</span></span>|<span data-ttu-id="551cb-115">Win32 业务线（LoB）应用程序的产品代码。</span><span class="sxs-lookup"><span data-stu-id="551cb-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="551cb-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="551cb-116">productVersionOperator</span></span>|[<span data-ttu-id="551cb-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="551cb-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="551cb-118">用于检测产品版本的运算符。</span><span class="sxs-lookup"><span data-stu-id="551cb-118">The operator to detect product version.</span></span> <span data-ttu-id="551cb-119">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="551cb-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="551cb-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="551cb-120">productVersion</span></span>|<span data-ttu-id="551cb-121">String</span><span class="sxs-lookup"><span data-stu-id="551cb-121">String</span></span>|<span data-ttu-id="551cb-122">Win32 业务线（LoB）应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="551cb-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="551cb-123">关系</span><span class="sxs-lookup"><span data-stu-id="551cb-123">Relationships</span></span>
<span data-ttu-id="551cb-124">无</span><span class="sxs-lookup"><span data-stu-id="551cb-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="551cb-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="551cb-125">JSON Representation</span></span>
<span data-ttu-id="551cb-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="551cb-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeDetection",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```



