---
title: importedWindowsAutopilotDeviceIdentityUpload 资源类型
description: 导入 windows 自动执行某些操作设备使用上载。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ea2c2620bf76410aa55d2568c6962fbb96636e3e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394724"
---
# <a name="importedwindowsautopilotdeviceidentityupload-resource-type"></a><span data-ttu-id="94f52-103">importedWindowsAutopilotDeviceIdentityUpload 资源类型</span><span class="sxs-lookup"><span data-stu-id="94f52-103">importedWindowsAutopilotDeviceIdentityUpload resource type</span></span>

> <span data-ttu-id="94f52-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="94f52-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="94f52-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="94f52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94f52-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94f52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94f52-107">导入 windows 自动执行某些操作设备使用上载。</span><span class="sxs-lookup"><span data-stu-id="94f52-107">Import windows autopilot devices using upload.</span></span>

## <a name="methods"></a><span data-ttu-id="94f52-108">方法</span><span class="sxs-lookup"><span data-stu-id="94f52-108">Methods</span></span>
|<span data-ttu-id="94f52-109">方法</span><span class="sxs-lookup"><span data-stu-id="94f52-109">Method</span></span>|<span data-ttu-id="94f52-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="94f52-110">Return Type</span></span>|<span data-ttu-id="94f52-111">说明</span><span class="sxs-lookup"><span data-stu-id="94f52-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="94f52-112">列表 importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="94f52-112">List importedWindowsAutopilotDeviceIdentityUploads</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-list.md)|<span data-ttu-id="94f52-113">[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)集合</span><span class="sxs-lookup"><span data-stu-id="94f52-113">[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) collection</span></span>|<span data-ttu-id="94f52-114">列出属性和[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="94f52-114">List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>|
|[<span data-ttu-id="94f52-115">获取 importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="94f52-115">Get importedWindowsAutopilotDeviceIdentityUpload</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-get.md)|[<span data-ttu-id="94f52-116">importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="94f52-116">importedWindowsAutopilotDeviceIdentityUpload</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|<span data-ttu-id="94f52-117">读取属性和[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="94f52-117">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>|
|[<span data-ttu-id="94f52-118">创建 importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="94f52-118">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-create.md)|[<span data-ttu-id="94f52-119">importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="94f52-119">importedWindowsAutopilotDeviceIdentityUpload</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|<span data-ttu-id="94f52-120">创建新的[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94f52-120">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>|
|[<span data-ttu-id="94f52-121">删除 importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="94f52-121">Delete importedWindowsAutopilotDeviceIdentityUpload</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-delete.md)|<span data-ttu-id="94f52-122">无</span><span class="sxs-lookup"><span data-stu-id="94f52-122">None</span></span>|<span data-ttu-id="94f52-123">删除[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)。</span><span class="sxs-lookup"><span data-stu-id="94f52-123">Deletes a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>|
|[<span data-ttu-id="94f52-124">更新 importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="94f52-124">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-update.md)|[<span data-ttu-id="94f52-125">importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="94f52-125">importedWindowsAutopilotDeviceIdentityUpload</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|<span data-ttu-id="94f52-126">更新[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94f52-126">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>|
|[<span data-ttu-id="94f52-127">autopilotDeviceStream 函数</span><span class="sxs-lookup"><span data-stu-id="94f52-127">autopilotDeviceStream function</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream.md)|<span data-ttu-id="94f52-128">String</span><span class="sxs-lookup"><span data-stu-id="94f52-128">String</span></span>|<span data-ttu-id="94f52-129">创建自动执行某些操作设备流上载请求。</span><span class="sxs-lookup"><span data-stu-id="94f52-129">Create a upload request with autopilot device stream in it.</span></span>|

## <a name="properties"></a><span data-ttu-id="94f52-130">属性</span><span class="sxs-lookup"><span data-stu-id="94f52-130">Properties</span></span>
|<span data-ttu-id="94f52-131">属性</span><span class="sxs-lookup"><span data-stu-id="94f52-131">Property</span></span>|<span data-ttu-id="94f52-132">类型</span><span class="sxs-lookup"><span data-stu-id="94f52-132">Type</span></span>|<span data-ttu-id="94f52-133">说明</span><span class="sxs-lookup"><span data-stu-id="94f52-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94f52-134">id</span><span class="sxs-lookup"><span data-stu-id="94f52-134">id</span></span>|<span data-ttu-id="94f52-135">String</span><span class="sxs-lookup"><span data-stu-id="94f52-135">String</span></span>|<span data-ttu-id="94f52-136">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="94f52-136">The GUID for the object</span></span>|
|<span data-ttu-id="94f52-137">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="94f52-137">createdDateTimeUtc</span></span>|<span data-ttu-id="94f52-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94f52-138">DateTimeOffset</span></span>|<span data-ttu-id="94f52-139">创建实体时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="94f52-139">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="94f52-140">status</span><span class="sxs-lookup"><span data-stu-id="94f52-140">status</span></span>|[<span data-ttu-id="94f52-141">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="94f52-141">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="94f52-142">上载状态。</span><span class="sxs-lookup"><span data-stu-id="94f52-142">Upload status.</span></span> <span data-ttu-id="94f52-143">可取值为：`noUpload`、`pending`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="94f52-143">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94f52-144">Relationships</span><span class="sxs-lookup"><span data-stu-id="94f52-144">Relationships</span></span>
|<span data-ttu-id="94f52-145">关系</span><span class="sxs-lookup"><span data-stu-id="94f52-145">Relationship</span></span>|<span data-ttu-id="94f52-146">类型</span><span class="sxs-lookup"><span data-stu-id="94f52-146">Type</span></span>|<span data-ttu-id="94f52-147">说明</span><span class="sxs-lookup"><span data-stu-id="94f52-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94f52-148">deviceIdentities</span><span class="sxs-lookup"><span data-stu-id="94f52-148">deviceIdentities</span></span>|<span data-ttu-id="94f52-149">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94f52-149">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="94f52-150">作为此上载的一部分自动执行某些操作的所有设备的集合。</span><span class="sxs-lookup"><span data-stu-id="94f52-150">Collection of all Autopilot devices as a part of this upload.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94f52-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94f52-151">JSON Representation</span></span>
<span data-ttu-id="94f52-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94f52-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "String (identifier)",
  "createdDateTimeUtc": "String (timestamp)",
  "status": "String"
}
```




