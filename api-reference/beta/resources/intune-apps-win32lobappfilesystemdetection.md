---
title: win32LobAppFileSystemDetection 资源类型
description: 包含要检测 Win32 应用程序的文件或文件夹路径
ms.openlocfilehash: 914c4f550b480bf16b2048945e66542311653338
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048012"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="a5a43-103">win32LobAppFileSystemDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5a43-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="a5a43-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a5a43-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5a43-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a5a43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5a43-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a5a43-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5a43-107">包含要检测 Win32 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="a5a43-107">Contains file or folder path to detect a Win32 App</span></span>

<span data-ttu-id="a5a43-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="a5a43-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a5a43-109">属性</span><span class="sxs-lookup"><span data-stu-id="a5a43-109">Properties</span></span>
|<span data-ttu-id="a5a43-110">属性</span><span class="sxs-lookup"><span data-stu-id="a5a43-110">Property</span></span>|<span data-ttu-id="a5a43-111">类型</span><span class="sxs-lookup"><span data-stu-id="a5a43-111">Type</span></span>|<span data-ttu-id="a5a43-112">说明</span><span class="sxs-lookup"><span data-stu-id="a5a43-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5a43-113">路径</span><span class="sxs-lookup"><span data-stu-id="a5a43-113">path</span></span>|<span data-ttu-id="a5a43-114">字符串</span><span class="sxs-lookup"><span data-stu-id="a5a43-114">String</span></span>|<span data-ttu-id="a5a43-115">要检测 Win32 业务线 (LoB) 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="a5a43-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="a5a43-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="a5a43-116">fileOrFolderName</span></span>|<span data-ttu-id="a5a43-117">字符串</span><span class="sxs-lookup"><span data-stu-id="a5a43-117">String</span></span>|<span data-ttu-id="a5a43-118">要检测 Win32 业务线 (LoB) 应用程序的文件或文件夹名称</span><span class="sxs-lookup"><span data-stu-id="a5a43-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="a5a43-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="a5a43-119">check32BitOn64System</span></span>|<span data-ttu-id="a5a43-120">布尔</span><span class="sxs-lookup"><span data-stu-id="a5a43-120">Boolean</span></span>|<span data-ttu-id="a5a43-121">一个值，该值此文件或文件夹是否检查 64 位系统上的 32 位应用程序</span><span class="sxs-lookup"><span data-stu-id="a5a43-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="a5a43-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="a5a43-122">detectionType</span></span>|[<span data-ttu-id="a5a43-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="a5a43-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="a5a43-124">文件系统检测类型。</span><span class="sxs-lookup"><span data-stu-id="a5a43-124">The file system detection type.</span></span> <span data-ttu-id="a5a43-125">可取值为：`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`。</span><span class="sxs-lookup"><span data-stu-id="a5a43-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="a5a43-126">operator</span><span class="sxs-lookup"><span data-stu-id="a5a43-126">operator</span></span>|[<span data-ttu-id="a5a43-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="a5a43-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="a5a43-128">文件或文件夹移检测运算符。</span><span class="sxs-lookup"><span data-stu-id="a5a43-128">The operator for file or fodler detection.</span></span> <span data-ttu-id="a5a43-129">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="a5a43-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="a5a43-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="a5a43-130">detectionValue</span></span>|<span data-ttu-id="a5a43-131">字符串</span><span class="sxs-lookup"><span data-stu-id="a5a43-131">String</span></span>|<span data-ttu-id="a5a43-132">文件或文件夹检测值</span><span class="sxs-lookup"><span data-stu-id="a5a43-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5a43-133">Relationships</span><span class="sxs-lookup"><span data-stu-id="a5a43-133">Relationships</span></span>
<span data-ttu-id="a5a43-134">无</span><span class="sxs-lookup"><span data-stu-id="a5a43-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a5a43-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5a43-135">JSON Representation</span></span>
<span data-ttu-id="a5a43-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5a43-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```





