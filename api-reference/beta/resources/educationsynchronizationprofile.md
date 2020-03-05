---
title: educationSynchronizationProfile 资源类型
description: 表示一组用于将源目录中的教育实体和名单信息同步到 Azure Active Directory （Azure AD）的配置。 此资源提供在学校数据同步中使用的编程表示形式。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7cea993bfaeaf7de82268747518288aaac836198
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500084"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="1eb44-104">educationSynchronizationProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="1eb44-104">educationSynchronizationProfile resource type</span></span>

<span data-ttu-id="1eb44-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1eb44-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1eb44-106">表示一组用于将源目录中的教育实体和名单信息同步到 Azure Active Directory （Azure AD）的配置。</span><span class="sxs-lookup"><span data-stu-id="1eb44-106">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="1eb44-107">此资源提供在[学校数据同步](https://sds.microsoft.com)中使用的编程表示形式。</span><span class="sxs-lookup"><span data-stu-id="1eb44-107">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="1eb44-108">方法</span><span class="sxs-lookup"><span data-stu-id="1eb44-108">Methods</span></span>

| <span data-ttu-id="1eb44-109">方法</span><span class="sxs-lookup"><span data-stu-id="1eb44-109">Method</span></span> | <span data-ttu-id="1eb44-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1eb44-110">Return Type</span></span> | <span data-ttu-id="1eb44-111">说明</span><span class="sxs-lookup"><span data-stu-id="1eb44-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="1eb44-112">列出同步配置文件</span><span class="sxs-lookup"><span data-stu-id="1eb44-112">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md) | <span data-ttu-id="1eb44-113">**educationSynchronizationProfile**集合</span><span class="sxs-lookup"><span data-stu-id="1eb44-113">**educationSynchronizationProfile** collection</span></span> | <span data-ttu-id="1eb44-114">获取租户中所有同步配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="1eb44-114">Get a list of all the synchronization profiles in the tenant.</span></span> |
| [<span data-ttu-id="1eb44-115">获取同步配置文件</span><span class="sxs-lookup"><span data-stu-id="1eb44-115">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md) | <span data-ttu-id="1eb44-116">**educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="1eb44-116">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="1eb44-117">在给定配置文件标识符的情况检索特定配置文件。</span><span class="sxs-lookup"><span data-stu-id="1eb44-117">Retrieve a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="1eb44-118">创建同步配置文件</span><span class="sxs-lookup"><span data-stu-id="1eb44-118">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md) | <span data-ttu-id="1eb44-119">无</span><span class="sxs-lookup"><span data-stu-id="1eb44-119">None</span></span> | <span data-ttu-id="1eb44-120">创建新的同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="1eb44-120">Create a new synchronization profile.</span></span> |
| [<span data-ttu-id="1eb44-121">删除同步配置文件</span><span class="sxs-lookup"><span data-stu-id="1eb44-121">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md) | <span data-ttu-id="1eb44-122">**educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="1eb44-122">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="1eb44-123">在给定配置文件标识符的情况删除特定配置文件。</span><span class="sxs-lookup"><span data-stu-id="1eb44-123">Delete a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="1eb44-124">暂停正在进行的同步</span><span class="sxs-lookup"><span data-stu-id="1eb44-124">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md) | <span data-ttu-id="1eb44-125">无</span><span class="sxs-lookup"><span data-stu-id="1eb44-125">None</span></span> | <span data-ttu-id="1eb44-126">暂停正在进行的同步。</span><span class="sxs-lookup"><span data-stu-id="1eb44-126">Pause an ongoing synchronization.</span></span> |
| [<span data-ttu-id="1eb44-127">恢复暂停的同步</span><span class="sxs-lookup"><span data-stu-id="1eb44-127">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md) | <span data-ttu-id="1eb44-128">无</span><span class="sxs-lookup"><span data-stu-id="1eb44-128">None</span></span> | <span data-ttu-id="1eb44-129">恢复暂停的同步。</span><span class="sxs-lookup"><span data-stu-id="1eb44-129">Resume a paused synchronization.</span></span> |
| [<span data-ttu-id="1eb44-130">重置同步</span><span class="sxs-lookup"><span data-stu-id="1eb44-130">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md) | <span data-ttu-id="1eb44-131">无</span><span class="sxs-lookup"><span data-stu-id="1eb44-131">None</span></span> | <span data-ttu-id="1eb44-132">重置配置文件的状态并重新启动同步。</span><span class="sxs-lookup"><span data-stu-id="1eb44-132">Reset the state of the profile and restart synchronization.</span></span> |
| [<span data-ttu-id="1eb44-133">开始同步上载的文件</span><span class="sxs-lookup"><span data-stu-id="1eb44-133">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) | <span data-ttu-id="1eb44-134">[educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md)集合</span><span class="sxs-lookup"><span data-stu-id="1eb44-134">[educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md) collection</span></span>| <span data-ttu-id="1eb44-135">验证上载的源文件并启动同步。</span><span class="sxs-lookup"><span data-stu-id="1eb44-135">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="1eb44-136">仅在数据提供程序为[educationCsvDataProvider](educationcsvdataprovider.md)时适用。</span><span class="sxs-lookup"><span data-stu-id="1eb44-136">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="1eb44-137">获取上载 URL</span><span class="sxs-lookup"><span data-stu-id="1eb44-137">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="1eb44-138">string</span><span class="sxs-lookup"><span data-stu-id="1eb44-138">string</span></span> | <span data-ttu-id="1eb44-139">返回短生存期的 URL 以上载 CSV 数据文件。</span><span class="sxs-lookup"><span data-stu-id="1eb44-139">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="1eb44-140">仅在数据提供程序为[educationCsvDataProvider](educationcsvdataprovider.md)时适用。</span><span class="sxs-lookup"><span data-stu-id="1eb44-140">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="1eb44-141">获取同步状态</span><span class="sxs-lookup"><span data-stu-id="1eb44-141">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | [<span data-ttu-id="1eb44-142">status</span><span class="sxs-lookup"><span data-stu-id="1eb44-142">status</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="1eb44-143">返回特定同步配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="1eb44-143">Return the status of a specific synchronization profile.</span></span> |
| [<span data-ttu-id="1eb44-144">获取同步错误</span><span class="sxs-lookup"><span data-stu-id="1eb44-144">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="1eb44-145">[educationSynchronizationError](educationsynchronizationerror.md)集合</span><span class="sxs-lookup"><span data-stu-id="1eb44-145">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="1eb44-146">获取同步过程中生成的所有错误。</span><span class="sxs-lookup"><span data-stu-id="1eb44-146">Get all the errors generated during synchronization.</span></span> |

## <a name="properties"></a><span data-ttu-id="1eb44-147">属性</span><span class="sxs-lookup"><span data-stu-id="1eb44-147">Properties</span></span>

| <span data-ttu-id="1eb44-148">属性</span><span class="sxs-lookup"><span data-stu-id="1eb44-148">Property</span></span> | <span data-ttu-id="1eb44-149">类型</span><span class="sxs-lookup"><span data-stu-id="1eb44-149">Type</span></span> | <span data-ttu-id="1eb44-150">说明</span><span class="sxs-lookup"><span data-stu-id="1eb44-150">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="1eb44-151">**displayName**</span><span class="sxs-lookup"><span data-stu-id="1eb44-151">**displayName**</span></span> | <span data-ttu-id="1eb44-152">string</span><span class="sxs-lookup"><span data-stu-id="1eb44-152">string</span></span> |  <span data-ttu-id="1eb44-153">用于同步标识的配置文件的名称。</span><span class="sxs-lookup"><span data-stu-id="1eb44-153">Name of the configuration profile for syncing identities.</span></span>         |
| <span data-ttu-id="1eb44-154">**dataProvider**</span><span class="sxs-lookup"><span data-stu-id="1eb44-154">**dataProvider**</span></span> | [<span data-ttu-id="1eb44-155">educationSynchronizationDataProvider</span><span class="sxs-lookup"><span data-stu-id="1eb44-155">educationSynchronizationDataProvider</span></span>](educationsynchronizationdataprovider.md) |  <span data-ttu-id="1eb44-156">用于配置文件的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="1eb44-156">The data provider used for the profile.</span></span>         |
| <span data-ttu-id="1eb44-157">**identitySynchronizationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="1eb44-157">**identitySynchronizationConfiguration**</span></span> | [<span data-ttu-id="1eb44-158">educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1eb44-158">educationIdentitySynchronizationConfiguration</span></span>](educationidentitysynchronizationconfiguration.md) | <span data-ttu-id="1eb44-159">标识的[创建](educationidentitycreationconfiguration.md)或[匹配](educationidentitymatchingconfiguration.md)配置。</span><span class="sxs-lookup"><span data-stu-id="1eb44-159">Identity [creation](educationidentitycreationconfiguration.md) or [matching](educationidentitymatchingconfiguration.md) configuration .</span></span>        |
| <span data-ttu-id="1eb44-160">**licensesToAssign**</span><span class="sxs-lookup"><span data-stu-id="1eb44-160">**licensesToAssign**</span></span> | <span data-ttu-id="1eb44-161">[educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1eb44-161">[educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md) collection</span></span>|  <span data-ttu-id="1eb44-162">许可证安装程序配置。</span><span class="sxs-lookup"><span data-stu-id="1eb44-162">License setup configuration.</span></span>        |
| <span data-ttu-id="1eb44-163">**state**</span><span class="sxs-lookup"><span data-stu-id="1eb44-163">**state**</span></span> | <span data-ttu-id="1eb44-164">educationSynchronizationProfileState</span><span class="sxs-lookup"><span data-stu-id="1eb44-164">educationSynchronizationProfileState</span></span> |  <span data-ttu-id="1eb44-165">配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="1eb44-165">The state of the profile.</span></span> <span data-ttu-id="1eb44-166">可取值为：`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed`。</span><span class="sxs-lookup"><span data-stu-id="1eb44-166">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span>          |

## <a name="relationships"></a><span data-ttu-id="1eb44-167">关系</span><span class="sxs-lookup"><span data-stu-id="1eb44-167">Relationships</span></span>

| <span data-ttu-id="1eb44-168">属性</span><span class="sxs-lookup"><span data-stu-id="1eb44-168">Property</span></span> | <span data-ttu-id="1eb44-169">类型</span><span class="sxs-lookup"><span data-stu-id="1eb44-169">Type</span></span> | <span data-ttu-id="1eb44-170">说明</span><span class="sxs-lookup"><span data-stu-id="1eb44-170">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="1eb44-171">**errors**</span><span class="sxs-lookup"><span data-stu-id="1eb44-171">**errors**</span></span> | <span data-ttu-id="1eb44-172">[educationSynchronizationError](educationsynchronizationerror.md)集合</span><span class="sxs-lookup"><span data-stu-id="1eb44-172">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="1eb44-173">与此同步配置文件关联的所有错误。</span><span class="sxs-lookup"><span data-stu-id="1eb44-173">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="1eb44-174">**profileStatus**</span><span class="sxs-lookup"><span data-stu-id="1eb44-174">**profileStatus**</span></span> | [<span data-ttu-id="1eb44-175">educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="1eb44-175">educationSynchronizationProfileStatus</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="1eb44-176">同步状态。</span><span class="sxs-lookup"><span data-stu-id="1eb44-176">The synchronization status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1eb44-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1eb44-177">JSON representation</span></span>
<span data-ttu-id="1eb44-178">下面是**educationSynchronizationProfile**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1eb44-178">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
    "id": "String",
    "displayName": "String",
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "microsoft.graph.educationCsvDataProvider" },
    "identitySynchronizationConfiguration": { "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```
