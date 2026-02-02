The dataset contains detailed metadata and download statistics for open-source AI models published on the Hugging Face Model Hub, enabling temporal, geographical, and modality-based analysis of the open model ecosystem.

Dataset Columns & Descriptions
```
_id – Unique identifier for each model record in the dataset.

model – Full model name and repository path on the Hugging Face Model Hub.

author – Original creator or publisher of the model.

time – Snapshot date representing when the download data was recorded.

created – Date and time when the model was first published on the Hub.

downloadsAllTime – Total cumulative number of downloads since the model’s release.

annotator – Entity type responsible for annotations (e.g., user, team, free).

org_model – Organization or entity associated with the model ownership.

org_type – Type of organization publishing the model (user, company, team).

org_country – Country or countries associated with the publishing organization.

derived_author – Standardized or inferred author name derived from metadata.

org_country_single – Primary country assigned to the organization.

derived_org_country – Cleaned or inferred organization country information.

derived_org_country_single – Single standardized country derived for consistency.

merged_country_groups_single – Grouped country classification for regional analysis.

merged_derived_country_groups_single – Region grouping based on derived country data.

merged_derived_from – Base or parent model(s) from which the current model is derived.

merged_languages – Supported language(s) of the model.

merged_modality – Input → output modality of the model (e.g., Text → Text, Image → Video).
```

Link : https://huggingface.co/datasets/mmpr/open_model_evolution_data/tree/main
