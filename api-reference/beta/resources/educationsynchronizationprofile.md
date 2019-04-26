---
title: educationSynchronizationProfile 资源类型
description: 表示一组用于将源目录中的教育实体和名单信息同步到 azure Active directory (azure AD) 的配置。 此资源提供在学校数据同步中使用的编程表示形式。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1926c591a679bd4fd97ceeeb7fab542af9e02544
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334042"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="60e41-104">educationSynchronizationProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="60e41-104">educationSynchronizationProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60e41-105">表示一组用于将源目录中的教育实体和名单信息同步到 azure Active directory (azure AD) 的配置。</span><span class="sxs-lookup"><span data-stu-id="60e41-105">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="60e41-106">此资源提供在[学校数据同步](https://sds.microsoft.com)中使用的编程表示形式。</span><span class="sxs-lookup"><span data-stu-id="60e41-106">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="60e41-107">方法</span><span class="sxs-lookup"><span data-stu-id="60e41-107">Methods</span></span>

| <span data-ttu-id="60e41-108">方法</span><span class="sxs-lookup"><span data-stu-id="60e41-108">Method</span></span> | <span data-ttu-id="60e41-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="60e41-109">Return Type</span></span> | <span data-ttu-id="60e41-110">说明</span><span class="sxs-lookup"><span data-stu-id="60e41-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="60e41-111">列出同步配置文件</span><span class="sxs-lookup"><span data-stu-id="60e41-111">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md) | <span data-ttu-id="60e41-112">**educationSynchronizationProfile**集合</span><span class="sxs-lookup"><span data-stu-id="60e41-112">**educationSynchronizationProfile** collection</span></span> | <span data-ttu-id="60e41-113">获取租户中所有同步配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="60e41-113">Get a list of all the synchronization profiles in the tenant.</span></span> |
| [<span data-ttu-id="60e41-114">获取同步配置文件</span><span class="sxs-lookup"><span data-stu-id="60e41-114">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md) | <span data-ttu-id="60e41-115">**educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="60e41-115">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="60e41-116">在给定配置文件标识符的情况检索特定配置文件。</span><span class="sxs-lookup"><span data-stu-id="60e41-116">Retrieve a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="60e41-117">创建同步配置文件</span><span class="sxs-lookup"><span data-stu-id="60e41-117">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md) | <span data-ttu-id="60e41-118">无</span><span class="sxs-lookup"><span data-stu-id="60e41-118">None</span></span> | <span data-ttu-id="60e41-119">创建新的同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="60e41-119">Create a new synchronization profile.</span></span> |
| [<span data-ttu-id="60e41-120">删除同步配置文件</span><span class="sxs-lookup"><span data-stu-id="60e41-120">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md) | <span data-ttu-id="60e41-121">**educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="60e41-121">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="60e41-122">在给定配置文件标识符的情况删除特定配置文件。</span><span class="sxs-lookup"><span data-stu-id="60e41-122">Delete a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="60e41-123">暂停正在进行的同步</span><span class="sxs-lookup"><span data-stu-id="60e41-123">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md) | <span data-ttu-id="60e41-124">无</span><span class="sxs-lookup"><span data-stu-id="60e41-124">None</span></span> | <span data-ttu-id="60e41-125">暂停正在进行的同步。</span><span class="sxs-lookup"><span data-stu-id="60e41-125">Pause an ongoing synchronization.</span></span> |
| [<span data-ttu-id="60e41-126">恢复暂停的同步</span><span class="sxs-lookup"><span data-stu-id="60e41-126">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md) | <span data-ttu-id="60e41-127">无</span><span class="sxs-lookup"><span data-stu-id="60e41-127">None</span></span> | <span data-ttu-id="60e41-128">恢复暂停的同步。</span><span class="sxs-lookup"><span data-stu-id="60e41-128">Resume a paused synchronization.</span></span> |
| [<span data-ttu-id="60e41-129">重置同步</span><span class="sxs-lookup"><span data-stu-id="60e41-129">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md) | <span data-ttu-id="60e41-130">无</span><span class="sxs-lookup"><span data-stu-id="60e41-130">None</span></span> | <span data-ttu-id="60e41-131">重置配置文件的状态并重新启动同步。</span><span class="sxs-lookup"><span data-stu-id="60e41-131">Reset the state of the profile and restart synchronization.</span></span> |
| [<span data-ttu-id="60e41-132">开始同步上载的文件</span><span class="sxs-lookup"><span data-stu-id="60e41-132">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) | <span data-ttu-id="60e41-133">[educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md)集合</span><span class="sxs-lookup"><span data-stu-id="60e41-133">[educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md) collection</span></span>| <span data-ttu-id="60e41-134">验证上载的源文件并启动同步。</span><span class="sxs-lookup"><span data-stu-id="60e41-134">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="60e41-135">仅在数据提供程序为[educationCsvDataProvider](educationcsvdataprovider.md)时适用。</span><span class="sxs-lookup"><span data-stu-id="60e41-135">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="60e41-136">获取上载 URL</span><span class="sxs-lookup"><span data-stu-id="60e41-136">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="60e41-137">string</span><span class="sxs-lookup"><span data-stu-id="60e41-137">string</span></span> | <span data-ttu-id="60e41-138">返回短生存期的 URL 以上载 CSV 数据文件。</span><span class="sxs-lookup"><span data-stu-id="60e41-138">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="60e41-139">仅在数据提供程序为[educationCsvDataProvider](educationcsvdataprovider.md)时适用。</span><span class="sxs-lookup"><span data-stu-id="60e41-139">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="60e41-140">获取同步状态</span><span class="sxs-lookup"><span data-stu-id="60e41-140">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | [<span data-ttu-id="60e41-141">status</span><span class="sxs-lookup"><span data-stu-id="60e41-141">status</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="60e41-142">返回特定同步配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="60e41-142">Return the status of a specific synchronization profile.</span></span> |
| [<span data-ttu-id="60e41-143">获取同步错误</span><span class="sxs-lookup"><span data-stu-id="60e41-143">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="60e41-144">[educationSynchronizationError](educationsynchronizationerror.md)集合</span><span class="sxs-lookup"><span data-stu-id="60e41-144">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="60e41-145">获取同步过程中生成的所有错误。</span><span class="sxs-lookup"><span data-stu-id="60e41-145">Get all the errors generated during synchronization.</span></span> |

## <a name="properties"></a><span data-ttu-id="60e41-146">属性</span><span class="sxs-lookup"><span data-stu-id="60e41-146">Properties</span></span>

| <span data-ttu-id="60e41-147">属性</span><span class="sxs-lookup"><span data-stu-id="60e41-147">Property</span></span> | <span data-ttu-id="60e41-148">类型</span><span class="sxs-lookup"><span data-stu-id="60e41-148">Type</span></span> | <span data-ttu-id="60e41-149">说明</span><span class="sxs-lookup"><span data-stu-id="60e41-149">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="60e41-150">**displayName**</span><span class="sxs-lookup"><span data-stu-id="60e41-150">**displayName**</span></span> | <span data-ttu-id="60e41-151">string</span><span class="sxs-lookup"><span data-stu-id="60e41-151">string</span></span> |  <span data-ttu-id="60e41-152">用于同步标识的配置文件的名称。</span><span class="sxs-lookup"><span data-stu-id="60e41-152">Name of the configuration profile for syncing identities.</span></span>         |
| <span data-ttu-id="60e41-153">**dataProvider**</span><span class="sxs-lookup"><span data-stu-id="60e41-153">**dataProvider**</span></span> | [<span data-ttu-id="60e41-154">educationSynchronizationDataProvider</span><span class="sxs-lookup"><span data-stu-id="60e41-154">educationSynchronizationDataProvider</span></span>](educationsynchronizationdataprovider.md) |  <span data-ttu-id="60e41-155">用于配置文件的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="60e41-155">The data provider used for the profile.</span></span>         |
| <span data-ttu-id="60e41-156">**identitySynchronizationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="60e41-156">**identitySynchronizationConfiguration**</span></span> | [<span data-ttu-id="60e41-157">educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="60e41-157">educationIdentitySynchronizationConfiguration</span></span>](educationidentitysynchronizationconfiguration.md) | <span data-ttu-id="60e41-158">标识的[创建](educationidentitycreationconfiguration.md)或[匹配](educationidentitymatchingconfiguration.md)配置。</span><span class="sxs-lookup"><span data-stu-id="60e41-158">Identity [creation](educationidentitycreationconfiguration.md) or [matching](educationidentitymatchingconfiguration.md) configuration .</span></span>        |
| <span data-ttu-id="60e41-159">**licensesToAssign**</span><span class="sxs-lookup"><span data-stu-id="60e41-159">**licensesToAssign**</span></span> | <span data-ttu-id="60e41-160">[educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="60e41-160">[educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md) collection</span></span>|  <span data-ttu-id="60e41-161">许可证安装程序配置。</span><span class="sxs-lookup"><span data-stu-id="60e41-161">License setup configuration.</span></span>        |
| <span data-ttu-id="60e41-162">**state**</span><span class="sxs-lookup"><span data-stu-id="60e41-162">**state**</span></span> | <span data-ttu-id="60e41-163">educationSynchronizationProfileState</span><span class="sxs-lookup"><span data-stu-id="60e41-163">educationSynchronizationProfileState</span></span> |  <span data-ttu-id="60e41-164">配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="60e41-164">The state of the profile.</span></span> <span data-ttu-id="60e41-165">可取值为：`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed`。</span><span class="sxs-lookup"><span data-stu-id="60e41-165">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span>          |

## <a name="relationships"></a><span data-ttu-id="60e41-166">Relationships</span><span class="sxs-lookup"><span data-stu-id="60e41-166">Relationships</span></span>

| <span data-ttu-id="60e41-167">属性</span><span class="sxs-lookup"><span data-stu-id="60e41-167">Property</span></span> | <span data-ttu-id="60e41-168">类型</span><span class="sxs-lookup"><span data-stu-id="60e41-168">Type</span></span> | <span data-ttu-id="60e41-169">说明</span><span class="sxs-lookup"><span data-stu-id="60e41-169">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="60e41-170">**errors**</span><span class="sxs-lookup"><span data-stu-id="60e41-170">**errors**</span></span> | <span data-ttu-id="60e41-171">[educationSynchronizationError](educationsynchronizationerror.md)集合</span><span class="sxs-lookup"><span data-stu-id="60e41-171">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="60e41-172">与此同步配置文件关联的所有错误。</span><span class="sxs-lookup"><span data-stu-id="60e41-172">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="60e41-173">**profileStatus**</span><span class="sxs-lookup"><span data-stu-id="60e41-173">**profileStatus**</span></span> | [<span data-ttu-id="60e41-174">educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="60e41-174">educationSynchronizationProfileStatus</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="60e41-175">同步状态。</span><span class="sxs-lookup"><span data-stu-id="60e41-175">The synchronization status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="60e41-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60e41-176">JSON representation</span></span>
<span data-ttu-id="60e41-177">下面是**educationSynchronizationProfile**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60e41-177">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

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
