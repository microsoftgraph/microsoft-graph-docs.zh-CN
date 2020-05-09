---
title: macOSAppleEventReceiver 资源类型
description: 表示可以接收 Apple 事件通知的过程。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 16064b1f7311f8ab384d7905a6f4cfa2f09ccc09
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177350"
---
# <a name="macosappleeventreceiver-resource-type"></a><span data-ttu-id="2b051-103">macOSAppleEventReceiver 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b051-103">macOSAppleEventReceiver resource type</span></span>

<span data-ttu-id="2b051-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b051-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b051-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2b051-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b051-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b051-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b051-107">表示可以接收 Apple 事件通知的过程。</span><span class="sxs-lookup"><span data-stu-id="2b051-107">Represents a process that can receive an Apple Event notification.</span></span>

## <a name="properties"></a><span data-ttu-id="2b051-108">属性</span><span class="sxs-lookup"><span data-stu-id="2b051-108">Properties</span></span>
|<span data-ttu-id="2b051-109">属性</span><span class="sxs-lookup"><span data-stu-id="2b051-109">Property</span></span>|<span data-ttu-id="2b051-110">类型</span><span class="sxs-lookup"><span data-stu-id="2b051-110">Type</span></span>|<span data-ttu-id="2b051-111">说明</span><span class="sxs-lookup"><span data-stu-id="2b051-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b051-112">codeRequirement</span><span class="sxs-lookup"><span data-stu-id="2b051-112">codeRequirement</span></span>|<span data-ttu-id="2b051-113">字符串</span><span class="sxs-lookup"><span data-stu-id="2b051-113">String</span></span>|<span data-ttu-id="2b051-114">接收 Apple 事件的应用程序或二进制文件的代码要求。</span><span class="sxs-lookup"><span data-stu-id="2b051-114">Code requirement for the app or binary that receives the Apple Event.</span></span>|
|<span data-ttu-id="2b051-115">标识符</span><span class="sxs-lookup"><span data-stu-id="2b051-115">identifier</span></span>|<span data-ttu-id="2b051-116">字符串</span><span class="sxs-lookup"><span data-stu-id="2b051-116">String</span></span>|<span data-ttu-id="2b051-117">接收 Apple 事件的进程或可执行文件的应用程序或文件路径的捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="2b051-117">Bundle ID of the app or file path of the process or executable that receives the Apple Event.</span></span>|
|<span data-ttu-id="2b051-118">identifierType</span><span class="sxs-lookup"><span data-stu-id="2b051-118">identifierType</span></span>|[<span data-ttu-id="2b051-119">macOSProcessIdentifierType</span><span class="sxs-lookup"><span data-stu-id="2b051-119">macOSProcessIdentifierType</span></span>](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|<span data-ttu-id="2b051-120">对接收 Apple 事件的进程或可执行文件使用应用程序或路径的捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="2b051-120">Use bundle ID for an app or path for a process or executable that receives the Apple Event.</span></span> <span data-ttu-id="2b051-121">可取值为：`bundleID`、`path`。</span><span class="sxs-lookup"><span data-stu-id="2b051-121">Possible values are: `bundleID`, `path`.</span></span>|
|<span data-ttu-id="2b051-122">支持</span><span class="sxs-lookup"><span data-stu-id="2b051-122">allowed</span></span>|<span data-ttu-id="2b051-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b051-123">Boolean</span></span>|<span data-ttu-id="2b051-124">允许或阻止此应用接收 Apple 事件。</span><span class="sxs-lookup"><span data-stu-id="2b051-124">Allow or block this app from receiving Apple events.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b051-125">关系</span><span class="sxs-lookup"><span data-stu-id="2b051-125">Relationships</span></span>
<span data-ttu-id="2b051-126">无</span><span class="sxs-lookup"><span data-stu-id="2b051-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b051-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b051-127">JSON Representation</span></span>
<span data-ttu-id="2b051-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b051-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAppleEventReceiver"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAppleEventReceiver",
  "codeRequirement": "String",
  "identifier": "String",
  "identifierType": "String",
  "allowed": true
}
```



