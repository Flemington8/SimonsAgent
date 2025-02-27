# NASDAQ100/SP500/SP400/DJIA History Companies Collection

## Requirements

```bash
pip install -r requirements.txt
```

## Collector Data
examples:
```bash
# parse instruments, using in qlib/instruments.
python collector.py --index_name NASDAQ100 --qlib_dir /root/onethingai-tmp/.qlib/qlib_data/us_data --method parse_instruments

python collector.py --index_name SP500 --qlib_dir /root/onethingai-tmp/.qlib/qlib_data/us_data --method parse_instruments

python collector.py --index_name DJIA --qlib_dir /root/onethingai-tmp/.qlib/qlib_data/us_data --method parse_instruments

python collector.py --index_name SP400 --qlib_dir /root/onethingai-tmp/.qlib/qlib_data/us_data --method parse_instruments

# parse new companies
python collector.py --index_name SP500 --qlib_dir /root/onethingai-tmp/.qlib/qlib_data/us_data --method save_new_companies

# index_name support: SP500, NASDAQ100, DJIA, SP400
# help
python collector.py --help
```

> **Note**: Since the data source is from the network outside the China mainland, we need to use a proxy to access the data. We modify the `collector.py` to support the proxy.