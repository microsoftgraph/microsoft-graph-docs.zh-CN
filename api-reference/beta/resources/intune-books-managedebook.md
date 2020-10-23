---
title: managedEBook 资源类型
description: 包含托管电子书基属性的抽象类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d303932765976cc8828fef5b256a7f7cf8e26482
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691482"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="d3a29-103">managedEBook 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3a29-103">managedEBook resource type</span></span>

<span data-ttu-id="d3a29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3a29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3a29-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3a29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3a29-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3a29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3a29-107">包含托管电子书基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="d3a29-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="d3a29-108">Methods</span><span class="sxs-lookup"><span data-stu-id="d3a29-108">Methods</span></span>
|<span data-ttu-id="d3a29-109">方法</span><span class="sxs-lookup"><span data-stu-id="d3a29-109">Method</span></span>|<span data-ttu-id="d3a29-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d3a29-110">Return Type</span></span>|<span data-ttu-id="d3a29-111">说明</span><span class="sxs-lookup"><span data-stu-id="d3a29-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d3a29-112">List managedEBooks</span><span class="sxs-lookup"><span data-stu-id="d3a29-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="d3a29-113">[managedEBook](../resources/intune-books-managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3a29-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="d3a29-114">列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3a29-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="d3a29-115">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="d3a29-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="d3a29-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="d3a29-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="d3a29-117">读取 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3a29-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="d3a29-118">assign 操作</span><span class="sxs-lookup"><span data-stu-id="d3a29-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="d3a29-119">无</span><span class="sxs-lookup"><span data-stu-id="d3a29-119">None</span></span>|<span data-ttu-id="d3a29-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d3a29-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d3a29-121">属性</span><span class="sxs-lookup"><span data-stu-id="d3a29-121">Properties</span></span>
|<span data-ttu-id="d3a29-122">属性</span><span class="sxs-lookup"><span data-stu-id="d3a29-122">Property</span></span>|<span data-ttu-id="d3a29-123">类型</span><span class="sxs-lookup"><span data-stu-id="d3a29-123">Type</span></span>|<span data-ttu-id="d3a29-124">说明</span><span class="sxs-lookup"><span data-stu-id="d3a29-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3a29-125">id</span><span class="sxs-lookup"><span data-stu-id="d3a29-125">id</span></span>|<span data-ttu-id="d3a29-126">String</span><span class="sxs-lookup"><span data-stu-id="d3a29-126">String</span></span>|<span data-ttu-id="d3a29-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d3a29-127">Key of the entity.</span></span>|
|<span data-ttu-id="d3a29-128">displayName</span><span class="sxs-lookup"><span data-stu-id="d3a29-128">displayName</span></span>|<span data-ttu-id="d3a29-129">String</span><span class="sxs-lookup"><span data-stu-id="d3a29-129">String</span></span>|<span data-ttu-id="d3a29-130">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="d3a29-130">Name of the eBook.</span></span>|
|<span data-ttu-id="d3a29-131">说明</span><span class="sxs-lookup"><span data-stu-id="d3a29-131">description</span></span>|<span data-ttu-id="d3a29-132">String</span><span class="sxs-lookup"><span data-stu-id="d3a29-132">String</span></span>|<span data-ttu-id="d3a29-133">说明。</span><span class="sxs-lookup"><span data-stu-id="d3a29-133">Description.</span></span>|
|<span data-ttu-id="d3a29-134">publisher</span><span class="sxs-lookup"><span data-stu-id="d3a29-134">publisher</span></span>|<span data-ttu-id="d3a29-135">String</span><span class="sxs-lookup"><span data-stu-id="d3a29-135">String</span></span>|<span data-ttu-id="d3a29-136">发布者。</span><span class="sxs-lookup"><span data-stu-id="d3a29-136">Publisher.</span></span>|
|<span data-ttu-id="d3a29-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3a29-137">publishedDateTime</span></span>|<span data-ttu-id="d3a29-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3a29-138">DateTimeOffset</span></span>|<span data-ttu-id="d3a29-139">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d3a29-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="d3a29-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="d3a29-140">largeCover</span></span>|[<span data-ttu-id="d3a29-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d3a29-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d3a29-142">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="d3a29-142">Book cover.</span></span>|
|<span data-ttu-id="d3a29-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3a29-143">createdDateTime</span></span>|<span data-ttu-id="d3a29-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3a29-144">DateTimeOffset</span></span>|<span data-ttu-id="d3a29-145">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d3a29-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="d3a29-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3a29-146">lastModifiedDateTime</span></span>|<span data-ttu-id="d3a29-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3a29-147">DateTimeOffset</span></span>|<span data-ttu-id="d3a29-148">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d3a29-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="d3a29-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d3a29-149">informationUrl</span></span>|<span data-ttu-id="d3a29-150">String</span><span class="sxs-lookup"><span data-stu-id="d3a29-150">String</span></span>|<span data-ttu-id="d3a29-151">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="d3a29-151">The more information Url.</span></span>|
|<span data-ttu-id="d3a29-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d3a29-152">privacyInformationUrl</span></span>|<span data-ttu-id="d3a29-153">String</span><span class="sxs-lookup"><span data-stu-id="d3a29-153">String</span></span>|<span data-ttu-id="d3a29-154">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="d3a29-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3a29-155">关系</span><span class="sxs-lookup"><span data-stu-id="d3a29-155">Relationships</span></span>
|<span data-ttu-id="d3a29-156">关系</span><span class="sxs-lookup"><span data-stu-id="d3a29-156">Relationship</span></span>|<span data-ttu-id="d3a29-157">类型</span><span class="sxs-lookup"><span data-stu-id="d3a29-157">Type</span></span>|<span data-ttu-id="d3a29-158">说明</span><span class="sxs-lookup"><span data-stu-id="d3a29-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3a29-159">类别</span><span class="sxs-lookup"><span data-stu-id="d3a29-159">categories</span></span>|<span data-ttu-id="d3a29-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3a29-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="d3a29-161">此电子书的类别列表。</span><span class="sxs-lookup"><span data-stu-id="d3a29-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="d3a29-162">assignments</span><span class="sxs-lookup"><span data-stu-id="d3a29-162">assignments</span></span>|<span data-ttu-id="d3a29-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3a29-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="d3a29-164">此电子书的分配列表。</span><span class="sxs-lookup"><span data-stu-id="d3a29-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="d3a29-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="d3a29-165">installSummary</span></span>|[<span data-ttu-id="d3a29-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d3a29-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="d3a29-167">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="d3a29-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="d3a29-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="d3a29-168">deviceStates</span></span>|<span data-ttu-id="d3a29-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3a29-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="d3a29-170">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="d3a29-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="d3a29-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="d3a29-171">userStateSummary</span></span>|<span data-ttu-id="d3a29-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3a29-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="d3a29-173">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="d3a29-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3a29-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3a29-174">JSON Representation</span></span>
<span data-ttu-id="d3a29-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3a29-175">Here is a JSON representation of the resource.</span></span>
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





