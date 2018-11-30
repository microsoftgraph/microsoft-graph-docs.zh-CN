---
title: win32LobAppMsiInformation 资源类型
description: Win32 应用程序包含 MSI 应用程序的属性。
ms.openlocfilehash: a5563d369d68a881f1b519c50dd9722ad864d7cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048676"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="63455-103">win32LobAppMsiInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="63455-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="63455-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="63455-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63455-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="63455-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63455-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="63455-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63455-107">Win32 应用程序包含 MSI 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="63455-107">Contains MSI app properties for a Win32 App.</span></span>
## <a name="properties"></a><span data-ttu-id="63455-108">属性</span><span class="sxs-lookup"><span data-stu-id="63455-108">Properties</span></span>
|<span data-ttu-id="63455-109">属性</span><span class="sxs-lookup"><span data-stu-id="63455-109">Property</span></span>|<span data-ttu-id="63455-110">类型</span><span class="sxs-lookup"><span data-stu-id="63455-110">Type</span></span>|<span data-ttu-id="63455-111">说明</span><span class="sxs-lookup"><span data-stu-id="63455-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63455-112">productCode</span><span class="sxs-lookup"><span data-stu-id="63455-112">productCode</span></span>|<span data-ttu-id="63455-113">String</span><span class="sxs-lookup"><span data-stu-id="63455-113">String</span></span>|<span data-ttu-id="63455-114">MSI 产品代码。</span><span class="sxs-lookup"><span data-stu-id="63455-114">The MSI product code.</span></span>|
|<span data-ttu-id="63455-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="63455-115">productVersion</span></span>|<span data-ttu-id="63455-116">String</span><span class="sxs-lookup"><span data-stu-id="63455-116">String</span></span>|<span data-ttu-id="63455-117">MSI 产品版本。</span><span class="sxs-lookup"><span data-stu-id="63455-117">The MSI product version.</span></span>|
|<span data-ttu-id="63455-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="63455-118">upgradeCode</span></span>|<span data-ttu-id="63455-119">字符串</span><span class="sxs-lookup"><span data-stu-id="63455-119">String</span></span>|<span data-ttu-id="63455-120">MSI 升级代码。</span><span class="sxs-lookup"><span data-stu-id="63455-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="63455-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="63455-121">requiresReboot</span></span>|<span data-ttu-id="63455-122">布尔</span><span class="sxs-lookup"><span data-stu-id="63455-122">Boolean</span></span>|<span data-ttu-id="63455-123">是否 MSI 应用程序要求计算机重新启动以完成安装。</span><span class="sxs-lookup"><span data-stu-id="63455-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="63455-124">： 键入包</span><span class="sxs-lookup"><span data-stu-id="63455-124">packageType</span></span>|[<span data-ttu-id="63455-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="63455-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="63455-126">MSI 包类型。</span><span class="sxs-lookup"><span data-stu-id="63455-126">The MSI package type.</span></span> <span data-ttu-id="63455-127">可取值为：`perMachine`、`perUser`、`dualPurpose`。</span><span class="sxs-lookup"><span data-stu-id="63455-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63455-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="63455-128">Relationships</span></span>
<span data-ttu-id="63455-129">无</span><span class="sxs-lookup"><span data-stu-id="63455-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="63455-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63455-130">JSON Representation</span></span>
<span data-ttu-id="63455-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63455-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String"
}
```





