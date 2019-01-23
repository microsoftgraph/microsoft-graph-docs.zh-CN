---
title: win32LobAppProductCodeDetection 资源类型
description: 包含产品代码和版本属性，以检测 Win32 应用程序
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f5af1cfc5fffe5241ef3b7883c3ebe6a2100278
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411202"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="97632-103">win32LobAppProductCodeDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="97632-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="97632-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="97632-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="97632-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="97632-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97632-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97632-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97632-107">包含产品代码和版本属性，以检测 Win32 应用程序</span><span class="sxs-lookup"><span data-stu-id="97632-107">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="97632-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="97632-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="97632-109">属性</span><span class="sxs-lookup"><span data-stu-id="97632-109">Properties</span></span>
|<span data-ttu-id="97632-110">属性</span><span class="sxs-lookup"><span data-stu-id="97632-110">Property</span></span>|<span data-ttu-id="97632-111">类型</span><span class="sxs-lookup"><span data-stu-id="97632-111">Type</span></span>|<span data-ttu-id="97632-112">说明</span><span class="sxs-lookup"><span data-stu-id="97632-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97632-113">productCode</span><span class="sxs-lookup"><span data-stu-id="97632-113">productCode</span></span>|<span data-ttu-id="97632-114">String</span><span class="sxs-lookup"><span data-stu-id="97632-114">String</span></span>|<span data-ttu-id="97632-115">Win32 业务线 (LoB) 应用程序的产品代码。</span><span class="sxs-lookup"><span data-stu-id="97632-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="97632-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="97632-116">productVersionOperator</span></span>|[<span data-ttu-id="97632-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="97632-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="97632-118">要检测产品版本的运算符。</span><span class="sxs-lookup"><span data-stu-id="97632-118">The operator to detect product version.</span></span> <span data-ttu-id="97632-119">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="97632-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="97632-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="97632-120">productVersion</span></span>|<span data-ttu-id="97632-121">String</span><span class="sxs-lookup"><span data-stu-id="97632-121">String</span></span>|<span data-ttu-id="97632-122">Win32 业务线 (LoB) 应用程序的产品版本。</span><span class="sxs-lookup"><span data-stu-id="97632-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97632-123">关系</span><span class="sxs-lookup"><span data-stu-id="97632-123">Relationships</span></span>
<span data-ttu-id="97632-124">无</span><span class="sxs-lookup"><span data-stu-id="97632-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97632-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97632-125">JSON Representation</span></span>
<span data-ttu-id="97632-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97632-126">Here is a JSON representation of the resource.</span></span>
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




