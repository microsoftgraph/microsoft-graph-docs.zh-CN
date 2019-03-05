---
title: win32LobAppProductCodeDetection 资源类型
description: 包含用于检测 Win32 应用程序的产品代码和版本属性
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 854d54b034b0e2e0dc0e7ce8e7f73466f37dd263
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173232"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="8c2b1-103">win32LobAppProductCodeDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c2b1-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="8c2b1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c2b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c2b1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c2b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c2b1-106">包含用于检测 Win32 应用程序的产品代码和版本属性</span><span class="sxs-lookup"><span data-stu-id="8c2b1-106">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="8c2b1-107">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="8c2b1-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c2b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c2b1-108">Properties</span></span>
|<span data-ttu-id="8c2b1-109">属性</span><span class="sxs-lookup"><span data-stu-id="8c2b1-109">Property</span></span>|<span data-ttu-id="8c2b1-110">类型</span><span class="sxs-lookup"><span data-stu-id="8c2b1-110">Type</span></span>|<span data-ttu-id="8c2b1-111">说明</span><span class="sxs-lookup"><span data-stu-id="8c2b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c2b1-112">productCode</span><span class="sxs-lookup"><span data-stu-id="8c2b1-112">productCode</span></span>|<span data-ttu-id="8c2b1-113">String</span><span class="sxs-lookup"><span data-stu-id="8c2b1-113">String</span></span>|<span data-ttu-id="8c2b1-114">Win32 业务线 (LoB) 应用程序的产品代码。</span><span class="sxs-lookup"><span data-stu-id="8c2b1-114">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8c2b1-115">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="8c2b1-115">productVersionOperator</span></span>|[<span data-ttu-id="8c2b1-116">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="8c2b1-116">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="8c2b1-117">用于检测产品版本的运算符。</span><span class="sxs-lookup"><span data-stu-id="8c2b1-117">The operator to detect product version.</span></span> <span data-ttu-id="8c2b1-118">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="8c2b1-118">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="8c2b1-119">productVersion</span><span class="sxs-lookup"><span data-stu-id="8c2b1-119">productVersion</span></span>|<span data-ttu-id="8c2b1-120">String</span><span class="sxs-lookup"><span data-stu-id="8c2b1-120">String</span></span>|<span data-ttu-id="8c2b1-121">Win32 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="8c2b1-121">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c2b1-122">关系</span><span class="sxs-lookup"><span data-stu-id="8c2b1-122">Relationships</span></span>
<span data-ttu-id="8c2b1-123">无</span><span class="sxs-lookup"><span data-stu-id="8c2b1-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c2b1-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c2b1-124">JSON Representation</span></span>
<span data-ttu-id="8c2b1-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c2b1-125">Here is a JSON representation of the resource.</span></span>
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




