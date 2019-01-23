---
title: adminConsent 资源类型
description: 管理许可信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c76ac169bb15792afec908f62b9740e81a4d7e5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415878"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="e2186-103">adminConsent 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2186-103">adminConsent resource type</span></span>

> <span data-ttu-id="e2186-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e2186-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e2186-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e2186-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2186-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2186-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2186-107">管理许可信息。</span><span class="sxs-lookup"><span data-stu-id="e2186-107">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="e2186-108">属性</span><span class="sxs-lookup"><span data-stu-id="e2186-108">Properties</span></span>
|<span data-ttu-id="e2186-109">属性</span><span class="sxs-lookup"><span data-stu-id="e2186-109">Property</span></span>|<span data-ttu-id="e2186-110">类型</span><span class="sxs-lookup"><span data-stu-id="e2186-110">Type</span></span>|<span data-ttu-id="e2186-111">说明</span><span class="sxs-lookup"><span data-stu-id="e2186-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2186-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="e2186-112">shareAPNSData</span></span>|[<span data-ttu-id="e2186-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="e2186-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="e2186-114">共享用户和设备数据到 Apple 管理员同意状态。</span><span class="sxs-lookup"><span data-stu-id="e2186-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="e2186-115">可取值为：`notConfigured`、`granted`、`notGranted`。</span><span class="sxs-lookup"><span data-stu-id="e2186-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2186-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="e2186-116">Relationships</span></span>
<span data-ttu-id="e2186-117">无</span><span class="sxs-lookup"><span data-stu-id="e2186-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2186-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2186-118">JSON Representation</span></span>
<span data-ttu-id="e2186-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2186-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```




