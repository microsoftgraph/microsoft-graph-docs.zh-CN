---
title: win32LobAppProductCodeDetection 资源类型
description: 包含产品代码和版本属性，以检测 Win32 应用程序
author: tfitzmac
ms.openlocfilehash: d66dab5a43a11c480e0e30f70eb8aecbe47e1fa7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353982"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="002d9-103">win32LobAppProductCodeDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="002d9-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="002d9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="002d9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="002d9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="002d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="002d9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="002d9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="002d9-107">包含产品代码和版本属性，以检测 Win32 应用程序</span><span class="sxs-lookup"><span data-stu-id="002d9-107">Contains product code and version properties to detect a Win32 App</span></span>

<span data-ttu-id="002d9-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="002d9-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="002d9-109">属性</span><span class="sxs-lookup"><span data-stu-id="002d9-109">Properties</span></span>
|<span data-ttu-id="002d9-110">属性</span><span class="sxs-lookup"><span data-stu-id="002d9-110">Property</span></span>|<span data-ttu-id="002d9-111">类型</span><span class="sxs-lookup"><span data-stu-id="002d9-111">Type</span></span>|<span data-ttu-id="002d9-112">说明</span><span class="sxs-lookup"><span data-stu-id="002d9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="002d9-113">productCode</span><span class="sxs-lookup"><span data-stu-id="002d9-113">productCode</span></span>|<span data-ttu-id="002d9-114">String</span><span class="sxs-lookup"><span data-stu-id="002d9-114">String</span></span>|<span data-ttu-id="002d9-115">Win32 业务线 (LoB) 应用程序的产品代码。</span><span class="sxs-lookup"><span data-stu-id="002d9-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="002d9-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="002d9-116">productVersionOperator</span></span>|[<span data-ttu-id="002d9-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="002d9-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="002d9-118">要检测产品版本的运算符。</span><span class="sxs-lookup"><span data-stu-id="002d9-118">The operator to detect product version.</span></span> <span data-ttu-id="002d9-119">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="002d9-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="002d9-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="002d9-120">productVersion</span></span>|<span data-ttu-id="002d9-121">String</span><span class="sxs-lookup"><span data-stu-id="002d9-121">String</span></span>|<span data-ttu-id="002d9-122">Win32 业务线 (LoB) 应用程序的产品版本。</span><span class="sxs-lookup"><span data-stu-id="002d9-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="002d9-123">Relationships</span><span class="sxs-lookup"><span data-stu-id="002d9-123">Relationships</span></span>
<span data-ttu-id="002d9-124">无</span><span class="sxs-lookup"><span data-stu-id="002d9-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="002d9-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="002d9-125">JSON Representation</span></span>
<span data-ttu-id="002d9-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="002d9-126">Here is a JSON representation of the resource.</span></span>
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





