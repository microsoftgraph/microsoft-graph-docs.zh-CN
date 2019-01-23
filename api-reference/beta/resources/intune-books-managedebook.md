---
title: managedEBook 资源类型
description: 包含托管电子书基属性的抽象类。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08bd5cc6f5630aca0ff5b35c5590875d259ad294
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422045"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="e2ec1-103">managedEBook 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2ec1-103">managedEBook resource type</span></span>

> <span data-ttu-id="e2ec1-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e2ec1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2ec1-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2ec1-107">包含托管电子书基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="e2ec1-108">方法</span><span class="sxs-lookup"><span data-stu-id="e2ec1-108">Methods</span></span>
|<span data-ttu-id="e2ec1-109">方法</span><span class="sxs-lookup"><span data-stu-id="e2ec1-109">Method</span></span>|<span data-ttu-id="e2ec1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2ec1-110">Return Type</span></span>|<span data-ttu-id="e2ec1-111">说明</span><span class="sxs-lookup"><span data-stu-id="e2ec1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e2ec1-112">List managedEBooks</span><span class="sxs-lookup"><span data-stu-id="e2ec1-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="e2ec1-113">[managedEBook](../resources/intune-books-managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2ec1-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="e2ec1-114">列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="e2ec1-115">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="e2ec1-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="e2ec1-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="e2ec1-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="e2ec1-117">读取 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="e2ec1-118">assign 操作</span><span class="sxs-lookup"><span data-stu-id="e2ec1-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="e2ec1-119">无</span><span class="sxs-lookup"><span data-stu-id="e2ec1-119">None</span></span>|<span data-ttu-id="e2ec1-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e2ec1-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e2ec1-121">属性</span><span class="sxs-lookup"><span data-stu-id="e2ec1-121">Properties</span></span>
|<span data-ttu-id="e2ec1-122">属性</span><span class="sxs-lookup"><span data-stu-id="e2ec1-122">Property</span></span>|<span data-ttu-id="e2ec1-123">类型</span><span class="sxs-lookup"><span data-stu-id="e2ec1-123">Type</span></span>|<span data-ttu-id="e2ec1-124">说明</span><span class="sxs-lookup"><span data-stu-id="e2ec1-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2ec1-125">id</span><span class="sxs-lookup"><span data-stu-id="e2ec1-125">id</span></span>|<span data-ttu-id="e2ec1-126">String</span><span class="sxs-lookup"><span data-stu-id="e2ec1-126">String</span></span>|<span data-ttu-id="e2ec1-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-127">Key of the entity.</span></span>|
|<span data-ttu-id="e2ec1-128">displayName</span><span class="sxs-lookup"><span data-stu-id="e2ec1-128">displayName</span></span>|<span data-ttu-id="e2ec1-129">String</span><span class="sxs-lookup"><span data-stu-id="e2ec1-129">String</span></span>|<span data-ttu-id="e2ec1-130">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-130">Name of the eBook.</span></span>|
|<span data-ttu-id="e2ec1-131">description</span><span class="sxs-lookup"><span data-stu-id="e2ec1-131">description</span></span>|<span data-ttu-id="e2ec1-132">String</span><span class="sxs-lookup"><span data-stu-id="e2ec1-132">String</span></span>|<span data-ttu-id="e2ec1-133">说明。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-133">Description.</span></span>|
|<span data-ttu-id="e2ec1-134">publisher</span><span class="sxs-lookup"><span data-stu-id="e2ec1-134">publisher</span></span>|<span data-ttu-id="e2ec1-135">String</span><span class="sxs-lookup"><span data-stu-id="e2ec1-135">String</span></span>|<span data-ttu-id="e2ec1-136">发布者。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-136">Publisher.</span></span>|
|<span data-ttu-id="e2ec1-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2ec1-137">publishedDateTime</span></span>|<span data-ttu-id="e2ec1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2ec1-138">DateTimeOffset</span></span>|<span data-ttu-id="e2ec1-139">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="e2ec1-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="e2ec1-140">largeCover</span></span>|[<span data-ttu-id="e2ec1-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e2ec1-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e2ec1-142">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-142">Book cover.</span></span>|
|<span data-ttu-id="e2ec1-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2ec1-143">createdDateTime</span></span>|<span data-ttu-id="e2ec1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2ec1-144">DateTimeOffset</span></span>|<span data-ttu-id="e2ec1-145">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="e2ec1-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2ec1-146">lastModifiedDateTime</span></span>|<span data-ttu-id="e2ec1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2ec1-147">DateTimeOffset</span></span>|<span data-ttu-id="e2ec1-148">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="e2ec1-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e2ec1-149">informationUrl</span></span>|<span data-ttu-id="e2ec1-150">String</span><span class="sxs-lookup"><span data-stu-id="e2ec1-150">String</span></span>|<span data-ttu-id="e2ec1-151">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-151">The more information Url.</span></span>|
|<span data-ttu-id="e2ec1-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e2ec1-152">privacyInformationUrl</span></span>|<span data-ttu-id="e2ec1-153">String</span><span class="sxs-lookup"><span data-stu-id="e2ec1-153">String</span></span>|<span data-ttu-id="e2ec1-154">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2ec1-155">关系</span><span class="sxs-lookup"><span data-stu-id="e2ec1-155">Relationships</span></span>
|<span data-ttu-id="e2ec1-156">关系</span><span class="sxs-lookup"><span data-stu-id="e2ec1-156">Relationship</span></span>|<span data-ttu-id="e2ec1-157">类型</span><span class="sxs-lookup"><span data-stu-id="e2ec1-157">Type</span></span>|<span data-ttu-id="e2ec1-158">说明</span><span class="sxs-lookup"><span data-stu-id="e2ec1-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2ec1-159">categories</span><span class="sxs-lookup"><span data-stu-id="e2ec1-159">categories</span></span>|<span data-ttu-id="e2ec1-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="e2ec1-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="e2ec1-161">此电子图书类别列表。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="e2ec1-162">assignments</span><span class="sxs-lookup"><span data-stu-id="e2ec1-162">assignments</span></span>|<span data-ttu-id="e2ec1-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2ec1-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="e2ec1-164">此电子书的分配列表。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="e2ec1-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="e2ec1-165">installSummary</span></span>|[<span data-ttu-id="e2ec1-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e2ec1-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="e2ec1-167">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="e2ec1-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="e2ec1-168">deviceStates</span></span>|<span data-ttu-id="e2ec1-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2ec1-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="e2ec1-170">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="e2ec1-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="e2ec1-171">userStateSummary</span></span>|<span data-ttu-id="e2ec1-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2ec1-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="e2ec1-173">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2ec1-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2ec1-174">JSON Representation</span></span>
<span data-ttu-id="e2ec1-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2ec1-175">Here is a JSON representation of the resource.</span></span>
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




