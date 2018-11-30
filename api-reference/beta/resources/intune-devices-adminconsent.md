---
title: adminConsent 资源类型
description: 管理许可信息。
ms.openlocfilehash: da7197c995d9c87ab69db11ae0c6c0804482877d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046294"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="fbe7d-103">adminConsent 资源类型</span><span class="sxs-lookup"><span data-stu-id="fbe7d-103">adminConsent resource type</span></span>

> <span data-ttu-id="fbe7d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fbe7d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbe7d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fbe7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbe7d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fbe7d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbe7d-107">管理许可信息。</span><span class="sxs-lookup"><span data-stu-id="fbe7d-107">Admin consent information.</span></span>
## <a name="properties"></a><span data-ttu-id="fbe7d-108">属性</span><span class="sxs-lookup"><span data-stu-id="fbe7d-108">Properties</span></span>
|<span data-ttu-id="fbe7d-109">属性</span><span class="sxs-lookup"><span data-stu-id="fbe7d-109">Property</span></span>|<span data-ttu-id="fbe7d-110">类型</span><span class="sxs-lookup"><span data-stu-id="fbe7d-110">Type</span></span>|<span data-ttu-id="fbe7d-111">说明</span><span class="sxs-lookup"><span data-stu-id="fbe7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbe7d-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="fbe7d-112">shareAPNSData</span></span>|[<span data-ttu-id="fbe7d-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="fbe7d-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="fbe7d-114">共享用户和设备数据到 Apple 管理员同意状态。</span><span class="sxs-lookup"><span data-stu-id="fbe7d-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="fbe7d-115">可取值为：`notConfigured`、`granted`、`notGranted`。</span><span class="sxs-lookup"><span data-stu-id="fbe7d-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbe7d-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="fbe7d-116">Relationships</span></span>
<span data-ttu-id="fbe7d-117">无</span><span class="sxs-lookup"><span data-stu-id="fbe7d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fbe7d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fbe7d-118">JSON Representation</span></span>
<span data-ttu-id="fbe7d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbe7d-119">Here is a JSON representation of the resource.</span></span>
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





