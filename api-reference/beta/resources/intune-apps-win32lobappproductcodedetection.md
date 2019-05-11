---
title: win32LobAppProductCodeDetection 资源类型
description: 包含用于检测 Win32 应用程序的产品代码和版本属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c56e3047ccc83e7d417e03bc4a95a8538650341
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949519"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="9f8e6-103">win32LobAppProductCodeDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f8e6-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="9f8e6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f8e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f8e6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f8e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f8e6-106">包含用于检测 Win32 应用程序的产品代码和版本属性</span><span class="sxs-lookup"><span data-stu-id="9f8e6-106">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="9f8e6-107">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="9f8e6-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9f8e6-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f8e6-108">Properties</span></span>
|<span data-ttu-id="9f8e6-109">属性</span><span class="sxs-lookup"><span data-stu-id="9f8e6-109">Property</span></span>|<span data-ttu-id="9f8e6-110">类型</span><span class="sxs-lookup"><span data-stu-id="9f8e6-110">Type</span></span>|<span data-ttu-id="9f8e6-111">说明</span><span class="sxs-lookup"><span data-stu-id="9f8e6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f8e6-112">productCode</span><span class="sxs-lookup"><span data-stu-id="9f8e6-112">productCode</span></span>|<span data-ttu-id="9f8e6-113">String</span><span class="sxs-lookup"><span data-stu-id="9f8e6-113">String</span></span>|<span data-ttu-id="9f8e6-114">Win32 业务线 (LoB) 应用程序的产品代码。</span><span class="sxs-lookup"><span data-stu-id="9f8e6-114">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9f8e6-115">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="9f8e6-115">productVersionOperator</span></span>|[<span data-ttu-id="9f8e6-116">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="9f8e6-116">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="9f8e6-117">用于检测产品版本的运算符。</span><span class="sxs-lookup"><span data-stu-id="9f8e6-117">The operator to detect product version.</span></span> <span data-ttu-id="9f8e6-118">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="9f8e6-118">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="9f8e6-119">productVersion</span><span class="sxs-lookup"><span data-stu-id="9f8e6-119">productVersion</span></span>|<span data-ttu-id="9f8e6-120">String</span><span class="sxs-lookup"><span data-stu-id="9f8e6-120">String</span></span>|<span data-ttu-id="9f8e6-121">Win32 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="9f8e6-121">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f8e6-122">关系</span><span class="sxs-lookup"><span data-stu-id="9f8e6-122">Relationships</span></span>
<span data-ttu-id="9f8e6-123">无</span><span class="sxs-lookup"><span data-stu-id="9f8e6-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f8e6-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f8e6-124">JSON Representation</span></span>
<span data-ttu-id="9f8e6-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f8e6-125">Here is a JSON representation of the resource.</span></span>
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




