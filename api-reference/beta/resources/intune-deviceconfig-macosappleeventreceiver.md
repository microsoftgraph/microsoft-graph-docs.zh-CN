---
title: macOSAppleEventReceiver 资源类型
description: 表示可以接收 Apple 事件通知的过程。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 073adb9d5a8668d825b3ee7d1fbd6f9fe35131fa
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693939"
---
# <a name="macosappleeventreceiver-resource-type"></a><span data-ttu-id="8c563-103">macOSAppleEventReceiver 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c563-103">macOSAppleEventReceiver resource type</span></span>

<span data-ttu-id="8c563-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c563-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c563-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c563-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c563-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c563-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c563-107">表示可以接收 Apple 事件通知的过程。</span><span class="sxs-lookup"><span data-stu-id="8c563-107">Represents a process that can receive an Apple Event notification.</span></span>

## <a name="properties"></a><span data-ttu-id="8c563-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c563-108">Properties</span></span>
|<span data-ttu-id="8c563-109">属性</span><span class="sxs-lookup"><span data-stu-id="8c563-109">Property</span></span>|<span data-ttu-id="8c563-110">类型</span><span class="sxs-lookup"><span data-stu-id="8c563-110">Type</span></span>|<span data-ttu-id="8c563-111">说明</span><span class="sxs-lookup"><span data-stu-id="8c563-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c563-112">codeRequirement</span><span class="sxs-lookup"><span data-stu-id="8c563-112">codeRequirement</span></span>|<span data-ttu-id="8c563-113">String</span><span class="sxs-lookup"><span data-stu-id="8c563-113">String</span></span>|<span data-ttu-id="8c563-114">接收 Apple 事件的应用程序或二进制文件的代码要求。</span><span class="sxs-lookup"><span data-stu-id="8c563-114">Code requirement for the app or binary that receives the Apple Event.</span></span>|
|<span data-ttu-id="8c563-115">标识符</span><span class="sxs-lookup"><span data-stu-id="8c563-115">identifier</span></span>|<span data-ttu-id="8c563-116">String</span><span class="sxs-lookup"><span data-stu-id="8c563-116">String</span></span>|<span data-ttu-id="8c563-117">接收 Apple 事件的进程或可执行文件的应用程序或文件路径的捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="8c563-117">Bundle ID of the app or file path of the process or executable that receives the Apple Event.</span></span>|
|<span data-ttu-id="8c563-118">identifierType</span><span class="sxs-lookup"><span data-stu-id="8c563-118">identifierType</span></span>|[<span data-ttu-id="8c563-119">macOSProcessIdentifierType</span><span class="sxs-lookup"><span data-stu-id="8c563-119">macOSProcessIdentifierType</span></span>](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|<span data-ttu-id="8c563-120">对接收 Apple 事件的进程或可执行文件使用应用程序或路径的捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="8c563-120">Use bundle ID for an app or path for a process or executable that receives the Apple Event.</span></span> <span data-ttu-id="8c563-121">可取值为：`bundleID`、`path`。</span><span class="sxs-lookup"><span data-stu-id="8c563-121">Possible values are: `bundleID`, `path`.</span></span>|
|<span data-ttu-id="8c563-122">支持</span><span class="sxs-lookup"><span data-stu-id="8c563-122">allowed</span></span>|<span data-ttu-id="8c563-123">布尔</span><span class="sxs-lookup"><span data-stu-id="8c563-123">Boolean</span></span>|<span data-ttu-id="8c563-124">允许或阻止此应用接收 Apple 事件。</span><span class="sxs-lookup"><span data-stu-id="8c563-124">Allow or block this app from receiving Apple events.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c563-125">关系</span><span class="sxs-lookup"><span data-stu-id="8c563-125">Relationships</span></span>
<span data-ttu-id="8c563-126">无</span><span class="sxs-lookup"><span data-stu-id="8c563-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c563-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c563-127">JSON Representation</span></span>
<span data-ttu-id="8c563-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c563-128">Here is a JSON representation of the resource.</span></span>
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





