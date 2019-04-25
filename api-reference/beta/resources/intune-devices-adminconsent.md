---
title: adminConsent 资源类型
description: 管理员同意信息。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b14eb19096a034612715081ae2e3dba25b5bb218
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534491"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="ed51b-103">adminConsent 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed51b-103">adminConsent resource type</span></span>

> <span data-ttu-id="ed51b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ed51b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed51b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed51b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed51b-106">管理员同意信息。</span><span class="sxs-lookup"><span data-stu-id="ed51b-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="ed51b-107">属性</span><span class="sxs-lookup"><span data-stu-id="ed51b-107">Properties</span></span>
|<span data-ttu-id="ed51b-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed51b-108">Property</span></span>|<span data-ttu-id="ed51b-109">类型</span><span class="sxs-lookup"><span data-stu-id="ed51b-109">Type</span></span>|<span data-ttu-id="ed51b-110">说明</span><span class="sxs-lookup"><span data-stu-id="ed51b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed51b-111">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="ed51b-111">shareAPNSData</span></span>|[<span data-ttu-id="ed51b-112">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="ed51b-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="ed51b-113">将用户和设备数据共享到 Apple 的管理员同意状态。</span><span class="sxs-lookup"><span data-stu-id="ed51b-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="ed51b-114">可取值为：`notConfigured`、`granted`、`notGranted`。</span><span class="sxs-lookup"><span data-stu-id="ed51b-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed51b-115">关系</span><span class="sxs-lookup"><span data-stu-id="ed51b-115">Relationships</span></span>
<span data-ttu-id="ed51b-116">无</span><span class="sxs-lookup"><span data-stu-id="ed51b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed51b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed51b-117">JSON Representation</span></span>
<span data-ttu-id="ed51b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed51b-118">Here is a JSON representation of the resource.</span></span>
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





