---
title: win32LobAppProductCodeDetection 资源类型
description: 包含产品代码和版本属性，以检测 Win32 应用程序
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a3a461661d2b2a37cd7f4e9a37561ea682ea0e0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812465"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="eb2f0-103">win32LobAppProductCodeDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb2f0-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="eb2f0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb2f0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb2f0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb2f0-107">包含产品代码和版本属性，以检测 Win32 应用程序</span><span class="sxs-lookup"><span data-stu-id="eb2f0-107">Contains product code and version properties to detect a Win32 App</span></span>

<span data-ttu-id="eb2f0-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="eb2f0-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb2f0-109">属性</span><span class="sxs-lookup"><span data-stu-id="eb2f0-109">Properties</span></span>
|<span data-ttu-id="eb2f0-110">属性</span><span class="sxs-lookup"><span data-stu-id="eb2f0-110">Property</span></span>|<span data-ttu-id="eb2f0-111">类型</span><span class="sxs-lookup"><span data-stu-id="eb2f0-111">Type</span></span>|<span data-ttu-id="eb2f0-112">Description</span><span class="sxs-lookup"><span data-stu-id="eb2f0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb2f0-113">productCode</span><span class="sxs-lookup"><span data-stu-id="eb2f0-113">productCode</span></span>|<span data-ttu-id="eb2f0-114">String</span><span class="sxs-lookup"><span data-stu-id="eb2f0-114">String</span></span>|<span data-ttu-id="eb2f0-115">Win32 业务线 (LoB) 应用程序的产品代码。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="eb2f0-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="eb2f0-116">productVersionOperator</span></span>|[<span data-ttu-id="eb2f0-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="eb2f0-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="eb2f0-118">要检测产品版本的运算符。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-118">The operator to detect product version.</span></span> <span data-ttu-id="eb2f0-119">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="eb2f0-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="eb2f0-120">productVersion</span></span>|<span data-ttu-id="eb2f0-121">String</span><span class="sxs-lookup"><span data-stu-id="eb2f0-121">String</span></span>|<span data-ttu-id="eb2f0-122">Win32 业务线 (LoB) 应用程序的产品版本。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb2f0-123">Relationships</span><span class="sxs-lookup"><span data-stu-id="eb2f0-123">Relationships</span></span>
<span data-ttu-id="eb2f0-124">无</span><span class="sxs-lookup"><span data-stu-id="eb2f0-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eb2f0-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb2f0-125">JSON Representation</span></span>
<span data-ttu-id="eb2f0-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-126">Here is a JSON representation of the resource.</span></span>
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





