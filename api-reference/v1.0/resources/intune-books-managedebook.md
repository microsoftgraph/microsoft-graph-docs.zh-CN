---
title: managedEBook 资源类型
description: 包含托管电子书基属性的抽象类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ee5bb486346e315ae00b0e54f44a9fd9b7613c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088669"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="8bef6-103">managedEBook 资源类型</span><span class="sxs-lookup"><span data-stu-id="8bef6-103">managedEBook resource type</span></span>

<span data-ttu-id="8bef6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bef6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8bef6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8bef6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bef6-106">包含托管电子书基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="8bef6-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="8bef6-107">方法</span><span class="sxs-lookup"><span data-stu-id="8bef6-107">Methods</span></span>
|<span data-ttu-id="8bef6-108">方法</span><span class="sxs-lookup"><span data-stu-id="8bef6-108">Method</span></span>|<span data-ttu-id="8bef6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8bef6-109">Return Type</span></span>|<span data-ttu-id="8bef6-110">说明</span><span class="sxs-lookup"><span data-stu-id="8bef6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8bef6-111">List managedEBooks</span><span class="sxs-lookup"><span data-stu-id="8bef6-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="8bef6-112">[managedEBook](../resources/intune-books-managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8bef6-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="8bef6-113">列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8bef6-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="8bef6-114">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="8bef6-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="8bef6-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="8bef6-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="8bef6-116">读取 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8bef6-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="8bef6-117">assign 操作</span><span class="sxs-lookup"><span data-stu-id="8bef6-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="8bef6-118">无</span><span class="sxs-lookup"><span data-stu-id="8bef6-118">None</span></span>|<span data-ttu-id="8bef6-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8bef6-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8bef6-120">属性</span><span class="sxs-lookup"><span data-stu-id="8bef6-120">Properties</span></span>
|<span data-ttu-id="8bef6-121">属性</span><span class="sxs-lookup"><span data-stu-id="8bef6-121">Property</span></span>|<span data-ttu-id="8bef6-122">类型</span><span class="sxs-lookup"><span data-stu-id="8bef6-122">Type</span></span>|<span data-ttu-id="8bef6-123">说明</span><span class="sxs-lookup"><span data-stu-id="8bef6-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bef6-124">id</span><span class="sxs-lookup"><span data-stu-id="8bef6-124">id</span></span>|<span data-ttu-id="8bef6-125">String</span><span class="sxs-lookup"><span data-stu-id="8bef6-125">String</span></span>|<span data-ttu-id="8bef6-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8bef6-126">Key of the entity.</span></span>|
|<span data-ttu-id="8bef6-127">displayName</span><span class="sxs-lookup"><span data-stu-id="8bef6-127">displayName</span></span>|<span data-ttu-id="8bef6-128">String</span><span class="sxs-lookup"><span data-stu-id="8bef6-128">String</span></span>|<span data-ttu-id="8bef6-129">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="8bef6-129">Name of the eBook.</span></span>|
|<span data-ttu-id="8bef6-130">description</span><span class="sxs-lookup"><span data-stu-id="8bef6-130">description</span></span>|<span data-ttu-id="8bef6-131">String</span><span class="sxs-lookup"><span data-stu-id="8bef6-131">String</span></span>|<span data-ttu-id="8bef6-132">说明。</span><span class="sxs-lookup"><span data-stu-id="8bef6-132">Description.</span></span>|
|<span data-ttu-id="8bef6-133">publisher</span><span class="sxs-lookup"><span data-stu-id="8bef6-133">publisher</span></span>|<span data-ttu-id="8bef6-134">String</span><span class="sxs-lookup"><span data-stu-id="8bef6-134">String</span></span>|<span data-ttu-id="8bef6-135">发布者。</span><span class="sxs-lookup"><span data-stu-id="8bef6-135">Publisher.</span></span>|
|<span data-ttu-id="8bef6-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bef6-136">publishedDateTime</span></span>|<span data-ttu-id="8bef6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bef6-137">DateTimeOffset</span></span>|<span data-ttu-id="8bef6-138">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8bef6-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="8bef6-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="8bef6-139">largeCover</span></span>|[<span data-ttu-id="8bef6-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8bef6-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8bef6-141">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="8bef6-141">Book cover.</span></span>|
|<span data-ttu-id="8bef6-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8bef6-142">createdDateTime</span></span>|<span data-ttu-id="8bef6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bef6-143">DateTimeOffset</span></span>|<span data-ttu-id="8bef6-144">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8bef6-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="8bef6-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bef6-145">lastModifiedDateTime</span></span>|<span data-ttu-id="8bef6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bef6-146">DateTimeOffset</span></span>|<span data-ttu-id="8bef6-147">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8bef6-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="8bef6-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8bef6-148">informationUrl</span></span>|<span data-ttu-id="8bef6-149">String</span><span class="sxs-lookup"><span data-stu-id="8bef6-149">String</span></span>|<span data-ttu-id="8bef6-150">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="8bef6-150">The more information Url.</span></span>|
|<span data-ttu-id="8bef6-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8bef6-151">privacyInformationUrl</span></span>|<span data-ttu-id="8bef6-152">String</span><span class="sxs-lookup"><span data-stu-id="8bef6-152">String</span></span>|<span data-ttu-id="8bef6-153">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="8bef6-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bef6-154">关系</span><span class="sxs-lookup"><span data-stu-id="8bef6-154">Relationships</span></span>
|<span data-ttu-id="8bef6-155">关系</span><span class="sxs-lookup"><span data-stu-id="8bef6-155">Relationship</span></span>|<span data-ttu-id="8bef6-156">类型</span><span class="sxs-lookup"><span data-stu-id="8bef6-156">Type</span></span>|<span data-ttu-id="8bef6-157">说明</span><span class="sxs-lookup"><span data-stu-id="8bef6-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bef6-158">assignments</span><span class="sxs-lookup"><span data-stu-id="8bef6-158">assignments</span></span>|<span data-ttu-id="8bef6-159">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8bef6-159">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="8bef6-160">此电子书的分配列表。</span><span class="sxs-lookup"><span data-stu-id="8bef6-160">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="8bef6-161">installSummary</span><span class="sxs-lookup"><span data-stu-id="8bef6-161">installSummary</span></span>|[<span data-ttu-id="8bef6-162">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="8bef6-162">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="8bef6-163">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="8bef6-163">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="8bef6-164">deviceStates</span><span class="sxs-lookup"><span data-stu-id="8bef6-164">deviceStates</span></span>|<span data-ttu-id="8bef6-165">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8bef6-165">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="8bef6-166">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="8bef6-166">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="8bef6-167">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="8bef6-167">userStateSummary</span></span>|<span data-ttu-id="8bef6-168">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8bef6-168">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="8bef6-169">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="8bef6-169">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bef6-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8bef6-170">JSON Representation</span></span>
<span data-ttu-id="8bef6-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bef6-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```









